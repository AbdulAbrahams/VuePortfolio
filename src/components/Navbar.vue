<template>

<nav class="navbar fixed-top my-2">
  <div class="container-fluid">
    <router-link class="navbar-brand" to="/"><img src="https://i.postimg.cc/66dv9ZGS/wahhaab-web-development-high-resolution-logo-color-on-transparent-background.png" width="125px" height="80px"></router-link>
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
            <router-link to="/" @click="scrollTop()"><a class="nav-link" href="#">Home</a></router-link>
          </li>
          <li class="nav-item">
            <router-link to="/about" @click="scrollTop()"><a class="nav-link" href="#">About</a></router-link>
          </li>
          <li class="nav-item">
            <router-link to="/resume" @click="scrollTop()"><a class="nav-link" href="#">Resume</a></router-link>
          </li>
          <li class="nav-item">
            <router-link to="/testimonials" @click="scrollTop()"><a class="nav-link" href="#">Testimonials</a></router-link>
          </li>
          <li class="nav-item">
            <router-link to="/projects" @click="scrollTop()"><a class="nav-link" href="#">Projects</a></router-link>
          </li>
          <li class="nav-item">
            <router-link to="/contact" @click="scrollTop()"><a class="nav-link" href="#">Contact</a></router-link>
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
      methods: {
      scrollTop() {
        document.body.scrollTop = document.documentElement.scrollTop = 0;
      }
    },
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

.navbar{
background: rgb(12, 12, 12);
}

nav {
  padding: 30px;
}

.navHead{
    color: orangered;
}

.navbar-toggler{
    border: 2px solid rgb(255, 0, 0) !important;
}

.toggler{
    font-size: 3vh;
    color: rgb(255, 0, 0);
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
  height: 50%;
}

.offcanvas-title{
  font-weight: bolder;
}
.offcanvas-body ul li a{
  color: black;
  width: 100%;
}
.offcanvas-body ul li :active {
  color: #ffffff;
}
.offcanvas-body ul li a:hover{
  color: rgb(220, 220, 220);
}
</style>
