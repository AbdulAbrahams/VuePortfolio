<template>
    <div class="resume">
    <h1 class="my-5">Resume</h1>
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
</template>

<script>
import Timeline from '../components/Timeline.vue'
import Skills from '../components/Skills.vue'
    export default {
        methods: {
      scrollTop() {
        document.body.scrollTop = document.documentElement.scrollTop = 0;
      }
    },
        name: 'Resume',
        components:{Timeline, Skills}
    }
</script>

<style scoped>
.resume{
    min-height: 100vh;
}
.resume h1{
    margin-top: 4%;
    color: red;
}

@media screen and (width <600px){
    .resume h1{
        margin-top: 20%;
    }
}
</style>
