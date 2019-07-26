<template>
  <section class="hero is-dark is-bold ">

  <!--  -->


  <carousel-3d :width="500" :height="300":controls-visible="true" :autoplay="true" :autoplay-timeout="5000" >
  <slide :index="0" >
    <img class="banner" src='../assets/Phuket-Fantasea.jpg'>
  </slide>
  <slide :index="1">
  <img class="banner" src='../assets/Safari-World.jpg'>
  </slide>
  <slide :index="2">
  <img class="banner" src='../assets/Sea-Life-Bangkok-Ocean-World.jpg'>
  </slide>
  <slide :index="3">
  <img class="banner" src='../assets/Chao-Pharaya-Princess.jpg'>
  </slide>
  <slide :index="4">
  <img class="banner" src='../assets/Chao-Pharaya-Princess.jpg'>
  </slide>
  <slide :index="5">
  <img class="banner" src='../assets/Chao-Pharaya-Princess.jpg'>
  </slide>


</carousel-3d>

 </section>
</template>

<script>


import { Carousel3d, Slide } from 'vue-carousel-3d';
export default {

  components: {
    Carousel3d,
    Slide
  }

};

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style >
.banner{



}


</style>
