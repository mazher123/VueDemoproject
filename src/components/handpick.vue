<template>


<section class="hero">

  <div class="hero-body">
    <div class="container handpick">

      <h2 class="">Handpicked Tours</h2>
      <p>Find only the best excursions here</P>
    </div>

    <div class="container">

       <tourcard-part v-bind:datas="datas"></tourcard-part>

        <div class="browse">
         <b-button size="is-medium" type="is-primary" outlined>Explore more</b-button>

       </div>

      </div>


    </div>






</section>





</template>

<script>
import tourcard from './tourcard.vue';
export default {

data (){

  return{

    datas: [
      {title: 'Safari world', place: 'Bangkok,Thailand', src:require('../assets/Chao-Pharaya-Princess.jpg')},
      {title: 'Sea life Ocean', place: 'Bangkok,Thailandy', src:require('../assets/Phuket-Fantasea.jpg')},
      {title: 'Phuket Fantase', place: 'Bangkok,Thailand',src:require('../assets/Safari-World.jpg')},
      {title: 'Chao Pharaya', place: 'Bangkok,Thailand', src:require('../assets/Sea-Life-Bangkok-Ocean-World.jpg')},

             ],

  }
},


  components:{

   'tourcard-part': tourcard


  }




}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style >
.handpick{

  margin-bottom: 20px;
}
  .handpick h2{
    font-family: "Lato", sans-serif;
    color: #484848;
    font-size: 32px;
  }

  .handpick p{
    margin: 0;
    font-size: 18px;
    color: #989898;
  }
.browse{

text-align: center;

}
.button.is-primary.is-outlined {
    background-color: transparent;
    border-color: #7957d5;
    color: #7957d5;
    width: 295px;
}

</style>
