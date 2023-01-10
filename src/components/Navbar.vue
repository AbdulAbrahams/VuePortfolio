<template>
    <!-- <nav>
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link> |
    <router-link to="/skills">Skills</router-link> |
    <router-link to="/resume">Resume</router-link> |
    <router-link to="/testimonials">Testimonials</router-link> |
    <router-link to="/contact">Contact</router-link>
  </nav> -->
  
  <!-- <div class="collapse" id="navbarToggleExternalContent">
  <div class="p-4">
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link> |
    <router-link to="/skills">Skills</router-link> |
    <router-link to="/resume">Resume</router-link> |
    <router-link to="/testimonials">Testimonials</router-link> |
    <router-link to="/contact">Contact</router-link>
  </div>
</div> -->
<nav class="navbar fixed-top my-2">
  <div class="container-fluid">
    <span class="navbar-brand"><img src="https://i.postimg.cc/66dv9ZGS/wahhaab-web-development-high-resolution-logo-color-on-transparent-background.png" width="125px" height="80px"></span>
    <button class="navbar-toggler" type="button" data-bs-toggle="offcanvas" data-bs-target="#offcanvasNavbar" aria-controls="offcanvasNavbar">
      <label class="toggler" for="toggle">☰</label>
    </button>
    <div class="offcanvas offcanvas-top" tabindex="-1" id="offcanvasNavbar" aria-labelledby="offcanvasNavbarLabel">
      <div class="offcanvas-header">
        <h5 class="offcanvas-title mx-3" id="offcanvasNavbarLabel" style="color:black">Wahhaab Web Development</h5>
        <button type="button" class="btn-close text-reset mx-5" data-bs-dismiss="offcanvas" aria-label="Close"></button>
      </div>
      <div class="offcanvas-body" data-bs-dismiss="offcanvas">
        <ul class="navbar-nav justify-content-end flex-grow-1 pe-3">
          <li class="nav-item">
            <a class="nav-link"><router-link to="/">Home</router-link></a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#"><router-link to="/about">About</router-link></a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#"> <router-link to="/resume">Resume</router-link> </a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#"><router-link to="/testimonials">Testimonials</router-link></a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#"><router-link to="/contact">Contact</router-link></a>
          </li>



        </ul>
      </div>
    </div>
  </div>
</nav>
<router-view/>
</template>

<script>
    export default {
       name: 'Navbar', 
    }
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

body{
  background: rgba(26, 26, 26, 0);
}

nav {
  padding: 30px;
}

.navHead{
    color: orangered;
}

.navbar-toggler{
    border: 2px solid orangered !important;
}

.toggler{
    font-size: 3vh;
    color: orangered;
}
nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}

.offcanvas{
  background-color: #7a1111;
  height: 45%;
}

</style>