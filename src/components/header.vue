<template>
  <!-- <div >




    <div class="hero is-primary">
     <div class="hero-body">
       <div class="container">




         <p class="is-size-3 has-text-centered">i am header</p>



       </div>
     </div>
    </div>

  </div> -->


<!-- <nav class="navbar" role="navigation" aria-label="main navigation">
  <div class="navbar ">
 <ul class="navbar-item">
    <li><b-icon icon="view-dashboard" size="is-medium" type="is-primary"></b-icon></li>
      <li class="navbar-end">gyugug</li>

</ul>




  </div>


</nav> -->


<nav class="navbar is-dark" role="navigation" aria-label="main navigation">
  <div class="navbar-brand">
    <a class="navbar-item" style="position: absolute; left: 50%; margin-left: -100px; margin-top: 0; padding: 0; height: 100%; display: flex; align-items: center;" href="https://bulma.io">
      <img src="../assets/logo.png">
    </a>

    <a role="button" class="navbar-burger burger" aria-label="menu" aria-expanded="false" data-target="navbarBasicExample">
      <span aria-hidden="true"></span>
      <span aria-hidden="true"></span>
      <span aria-hidden="true"></span>
    </a>
  </div>

  <div id="navbarBasicExample" class="navbar-menu">
    <div class="navbar-start">
      <a class="navbar-item">
        Home
      </a>

      <a class="navbar-item">
        Documentation
      </a>

      <div class="navbar-item has-dropdown is-hoverable">
        <a class="navbar-link">
          More
        </a>

        <div class="navbar-dropdown">
          <a class="navbar-item">
            About
          </a>
          <a class="navbar-item">
            Jobs
          </a>
          <a class="navbar-item">
            Contact
          </a>
          <hr class="navbar-divider">
          <a class="navbar-item">
            Report an issue
          </a>
        </div>
      </div>
    </div>

    <div class="navbar-end">
      <div class="navbar-item">
        <div class="buttons">

          <a class="button is-white">
          <i class="fas fa-search fa-1x"></i>
          </a>
        </div>
      </div>
    </div>
  </div>
</nav>


</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style >
.search{
  text-align: left;
}

</style>
