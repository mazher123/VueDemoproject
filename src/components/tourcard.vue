<template>
  <div class="columns">
    <!-- <div class="column">
      <div class="card ">
      <div class="card-image">
        <figure class="image is-4by3" id="img-hover-zoom">

          <img src='../assets/Chao-Pharaya-Princess.jpg' alt="Placeholder image">

        </figure>
      </div>
      <div class="card-content">

          <div class="media-content">

              <p class="is-size-5 is-bold">Safari World Ticket</p>
              <p class="is-size-6"><span  class="fa fa-map-marker" ></span> Bangkok,Thailand</p>
               <star-rating :stars="5" star-size="13"></star-rating>

        </div>

        <div class="content">
        </br>
          <p>BDT Tk 500</p>
          <br>
          <time datetime="2016-1-1">11:09 PM - 1 Jan 2016</time>
        </div>
      </div>
    </div>
    </div>
    <div class="column">
      <div class="card">
      <div class="card-image">
        <figure class="image is-4by3 " id="img-hover-zoom">
          <img src="../assets/Phuket-Fantasea.jpg" alt="Placeholder image">
        </figure>
      </div>
      <div class="card-content">

          <div class="media-content">

              <p class="is-size-5 is-bold">Safari World Ticket</p>
              <p class="is-size-6"><span  class="fa fa-map-marker" ></span> Bangkok,Thailand</p>
              <star-rating :stars="5"star-size="13"></star-rating>

        </div>

        <div class="content">
        </br>
          <p>BDT Tk 500</p>
          <br>
          <time datetime="2016-1-1">11:09 PM - 1 Jan 2016</time>
        </div>
      </div>
    </div>
    </div>
    <div class="column">
      <div class="card">
      <div class="card-image">
        <figure class="image is-4by3"  id="img-hover-zoom">
          <img src="../assets/Safari-World.jpg" alt="Placeholder image">
        </figure>
      </div>
      <div class="card-content">

          <div class="media-content">

              <p class="is-size-5 is-bold">Safari World Ticket</p>
              <p class="is-size-6"><span  class="fa fa-map-marker" ></span> Bangkok,Thailand</p>
                 <star-rating :stars="5" star-size="13"></star-rating>
        </div>

        <div class="content">
        </br>
          <p>BDT Tk 500</p>
          <br>
          <time datetime="2016-1-1">11:09 PM - 1 Jan 2016</time>
        </div>
      </div>
    </div>
    </div>
    <div class="column">
      <div class="card">
      <div class="card-image">
        <figure class="image is-4by3"  id="img-hover-zoom">
          <img src="../assets/Sea-Life-Bangkok-Ocean-World.jpg" alt="Placeholder image">
        </figure>
      </div>
      <div class="card-content">

          <div class="media-content">

              <p class="is-size-5 is-bold">Safari World Ticket</p>
              <p class="is-size-6"><span  class="fa fa-map-marker" ></span> Bangkok,Thailand</p>
                   <star-rating :stars="5" star-size="13"></star-rating>
        </div>

        <div class="content">
        </br>
          <p>BDT Tk 500</p>
          <br>
          <time datetime="2016-1-1">11:09 PM - 1 Jan 2016</time>
        </div>
      </div>
    </div>
    </div> -->


    <div class="column" v-for="data in datas">
      <div class="card ">
      <div class="card-image">
        <figure class="image is-4by3" id="img-hover-zoom">

          <img :src="data.src" alt="Placeholder image">

        </figure>
      </div>
      <div class="card-content">

          <div class="media-content">

              <p class="is-size-5 is-bold">{{data.title}}</p>
              <p class="is-size-6"><span  class="fa fa-map-marker" ></span>  {{data.place}}</p>
               <star-rating :stars="5" star-size="13"></star-rating>

        </div>

        <div class="content">
        </br>
          <p>BDT Tk 500</p>
          <br>
          <time datetime="2016-1-1">11:09 PM - 1 Jan 2016</time>
        </div>
      </div>
    </div>
    </div>






  </div>









</template>

<script>




export default {
props:{

  datas:{
    type:Array
  }
}



}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style >
#img-hover-zoom img{
  transition: transform .5s, filter 0.5s ease-in-out;
    filter: grayscale(80%);


}

#img-hover-zoom:hover img{
  filter: grayscale(0);
transform: scale(1.0);

}


</style>
