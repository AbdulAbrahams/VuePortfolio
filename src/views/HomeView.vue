<template>

<NavbarTwo/>

    <main class="homeBack">
    <div class="homes">
        <img src="https://iili.io/dH1seAx.gif">
        <h4>Web Developer</h4>
        <h1>Abdul Wahhaab Abrahams</h1>
        <button class="learnBtn btn">
            <router-link to="/about" style="text-decoration: none; color: red;" @click="scrollTop()"><a>Learn About Me</a></router-link>
        </button>
    </div>
    </main>

</template>

<script>

import NavbarTwo from '../components/NavbarTwo.vue'
export default{
  components: {NavbarTwo},
  
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
    width: 100vw;
    background-color: black;
}

.homes{
    top: 50%;
    left: 50%;
    position: absolute;
    transform: translate(-50%,-50%);
    box-sizing: border-box;
    width: 100vw;
}

.homeBack img{
    background-size: cover;
    position: relative;
    min-width: 40vw;
    max-width: 100%;
    max-height: 100%;
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
    border-radius: 0px;
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
</style>
