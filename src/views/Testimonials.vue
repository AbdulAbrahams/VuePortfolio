<template>

<div class="space"></div>
        <h1 style="color:red;">Testimonials</h1>
        <Card />


    <button class="BackNext1">
            <router-link to="/resume" @click="scrollTop()"><a>Back</a></router-link>
          </button>
          <button class="BackNext">
            <router-link to="/projects" @click="scrollTop()"><a>Next</a></router-link>
          </button>
</template>

<script>
import Card from '../components/Card.vue'
import Navbar from '../components/Navbar.vue'
import Footer from '../components/Footer.vue' 

export default {
        name: 'Testimonials',
        components:{Navbar, Footer, Card},
        
        methods: {
            scrollTop() {
                document.body.scrollTop = document.documentElement.scrollTop = 0;
               }
          },
    }
</script>

<style scoped>

.space{
    margin-top: 80px;
}


</style>
