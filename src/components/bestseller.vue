<template>



  <section class="hero  is-medium bestseller">

    <div class="hero-body">
      <div class="container handpick2">

        <h2 class="">Best Seller Tours</h2>
        <p>Find only the best excursions here</P>
      </div>
    <div class="container ">


     <hooper style="height: 600px"  :autoPlay="true" :playSpeed="2000">
          <slide>
          <tourcard-part v-bind:datas="datas"></tourcard-part>
          </slide>
          <slide>
          <tourcard-part v-bind:datas="datas"></tourcard-part>
          </slide>
          <slide>
          <tourcard-part v-bind:datas="datas"></tourcard-part>
          </slide>

        </hooper>

        <div class="browse">
         <b-button size="is-medium" type="is-warning" outlined><i class="fas fa-angle-double-down"></i></b-button>

       </div>

      </div>
    </div>


  </section>




  <!-- <div >

     <h2>i am best seller --</h2>
         <handpick-part></handpick-part>
          <tourcard-part></tourcard-part>

  </div> -->
</template>

<script>


 import handpick from './handpick.vue';
 import tourcard from './tourcard.vue';
 import { Hooper, Slide } from 'hooper';
 import 'hooper/dist/hooper.css';

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


 name: 'App',


  components:{

   'handpick-part': handpick,
    'tourcard-part': tourcard,
    Hooper,
    Slide



}
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style >
.handpick2{

  margin-bottom: 20px;
}
  .handpick2 h2{
    font-family: "Lato", sans-serif;
    color: #fff;
    font-size: 32px;
  }

  .handpick2 p{
    margin: 0;
    font-size: 18px;
    color: #989898;
  }
.bestseller{
  background-color: #081500f0;
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
