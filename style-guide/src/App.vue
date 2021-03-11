<template>
  <div id="app">
    <Btn>TEST</Btn>
  </div>
</template>

<script>
import Btn from "./components/Btn";
export default {
  name: "App",
  components: {
    Btn,
  },
};
</script>

<style lang="scss">
@import "./assets/main.scss";
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
