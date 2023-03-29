<template>

<Navbar2/>

    <main class="homeBack">
        <img src="https://i.postimg.cc/V6kJtpmG/d3cc6718eaa8898fba1e612e62511bd9.gif">
        <h4>Web Developer</h4>
        <h1>Abdul Wahhaab Abrahams</h1>
        <button class="learnBtn btn">
            <router-link to="/about" style="text-decoration: none; color: red;"><a>Learn About Me</a></router-link>
        </button>
    </main>

</template>

<script>

import Navbar from '../components/Navbar2.vue'
export default{
  name: Home
  components: {Navbar2},
  
    methods: {
      scrollTop() {
        document.body.scrollTop = document.documentElement.scrollTop = 0;
      }
    }
  }
</script>

<style>
.homeBack{
    min-height: 100vh;
    background-color: black;
}

.homeBack img{
    background-size: cover;
    position: relative;
    min-width: 40vw;
    max-width: 100%;
    max-height: 100%;
    margin-top: 6%;
}

.homeBack h4{
    color: white;
    top: 40%;
}

.homeBack h1{
    color: white;
}

.learnBtn{
    text-decoration: none;
    border: 2px solid red;
}

.learnBtn:hover{
    color: rgb(255, 255, 255) !important;
    background-color: rgb(255, 0, 0);
}

.learnBtn a:hover{
    width: 100%;
    height: 100%;
    color: white !important;

}

@media screen and (width <900px){
    .homeBack img{
        margin-top: 25%;
    }
}

@media screen and (width <550px){
    .homeBack img{
        margin-top: 60%;
    }
}
</style>
