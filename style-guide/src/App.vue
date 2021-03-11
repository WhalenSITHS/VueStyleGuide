<template>
  <div id="app" class="theme">
    <Btn color="primary">TEST</Btn>
    <Btn color="secondary">TEST</Btn>
    <HeaderOne>This is my header</HeaderOne>
  </div>
</template>

<script>
import Btn from "./components/Btn";
import HeaderOne from "./components/Header";
export default {
  name: "App",
  components: {
    Btn,
    HeaderOne,
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
