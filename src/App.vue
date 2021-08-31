<template>
  <div id="app">
    <TopBar />
    <Gallary />
    <EndBar />
  </div>
</template>

<script>
import TopBar from "./components/TopBar";
import EndBar from "./components/EndBar.vue";
import Gallary from "./components/Gallary.vue";

export default {
  name: "App",
  components: {
    TopBar,EndBar,Gallary,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
* {
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  box-sizing: border-box;
}

</style>
