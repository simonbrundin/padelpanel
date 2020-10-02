<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/totalpadel.png" class="logo" />

    <div class="activities">
      <div v-for="(aktivitet, index) in aktiviteter" class="aktivitetsrad">
        {{ aktivitet.rubrik }}
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      aktiviteter: [
        { rubrik: "Tävling", beskrivning: "Kalas tävling med magiska priser" },
        { rubrik: "Öppet hus", beskrivning: "Kom och prova på padel" },
      ],
    };
  },
};
</script>

<style>
body {
  background: #000;
}

#app {
  background: #000;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.logo {
  position: absolute;
  left: 0;
  top: 0;
  margin: 0 0 0 5vw;
}

.aktivitetsrad {
  color: white;
}
</style>
