<template>

<Navbar/>

   <div class="space"></div>
    <div class="resume">
    <h1>Resume</h1>
    <Timeline />
    <h1>Skills</h1>
    <Skills /> 
    </div>
         <button class="BackNext1">
            <router-link to="/about" @click="scrollTop()"><a>Back</a></router-link>
          </button>
          <button class="BackNext">
            <router-link to="/testimonials" @click="scrollTop()"><a>Next</a></router-link>
          </button>
          
<Footer/>          
</template>

<script>
import Timeline from '../components/Timeline.vue'
import Skills from '../components/Skills.vue'
import Navbar from '../components/Navbar.vue'
import Footer from '../components/Footer.vue' 

export default {
        name: 'Resume',
        components:{Navbar, Footer, Timeline, Skills},
        
        methods: {
            scrollTop() {
                document.body.scrollTop = document.documentElement.scrollTop = 0;
               }
          },
    }
</script>

<style scoped>
.resume{
    min-height: 100vh;
}
.resume h1{
    margin-top: 4%;
    color: red;
    font-size: 34px;
}

@media screen and (width <600px){
    .resume h1{
        margin-top: 20%;
    }
}
</style>
