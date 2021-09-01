<template>
  <div id="app">
    <TopBar />
    <CardInfo />
    <Gallary />
    <EndBar />
  </div>
</template>

<script>
import TopBar from "./components/TopBar";
import EndBar from "./components/EndBar.vue";
import Gallary from "./components/Gallary.vue";
import CardInfo from "./components/CardInfo.vue";

export default {
  name: "App",
  components: {
    TopBar,EndBar,Gallary,CardInfo,
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
body{
  margin-bottom:30px; 
}

</style>
