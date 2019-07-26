<template>

<div >
<header-part></header-part>

<banner-part></banner-part>
<handpick-part></handpick-part>
<bestseller-part></bestseller-part>
<footer-part></footer-part>





</div>



</template>


<script>
 import header from './components/header.vue';
 import banner from './components/banner.vue';
 import handpick from './components/handpick.vue';
 import bestseller from './components/bestseller.vue';
 import footer from './components/footer.vue';

 export default{

   components:{

    'header-part': header,
    'banner-part':banner,
    'handpick-part':handpick,
    'bestseller-part':bestseller,
  'footer-part':footer,


   },

   data(){

     return{

     }
   },

   methods:{

   }

 }





</script>









<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
#nav {
  padding: 30px;
  a {
    font-weight: bold;
    color: #2c3e50;
    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
