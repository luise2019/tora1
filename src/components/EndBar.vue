<template>
  <div class="EndBar">
    <footer class="end1">
      <H2>中间准备放点啥</H2>
    </footer>
  </div>
</template>

<script>
export default {
  name: "EndBar",
  components: {
    
  },
};
</script>

<style>
.end1 {
  width:100%;
  height: 30px;
  /* A gradient at the center of its container,
   starting red, changing to blue, and finishing green */
  background-image: radial-gradient(circle at center, pink 50%, cyan 100%);
  position: fixed;
  bottom:0;
}

</style>