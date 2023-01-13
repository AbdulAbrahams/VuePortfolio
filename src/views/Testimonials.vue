<template>
    <div class="space">
        <h1 style="color:red;">Testimonials</h1>
        <Card />
    </div>

    <button class="BackNext">
            <router-link to="/resume" @click="scrollTop()"><a>Back</a></router-link>
          </button>
          <button class="BackNext">
            <router-link to="/projects" @click="scrollTop()"><a>Next</a></router-link>
          </button>
</template>

<script>
import Card from '../components/Card.vue'
    export default {
        methods: {
      scrollTop() {
        document.body.scrollTop = document.documentElement.scrollTop = 0;
      }
    },
        name: 'Testimonials',
        components: {Card},
    }
</script>

<style scoped>

.space{
    margin-top: 5%;
}

@media screen and (width <600px){
    .space{
        margin-top: 20%;
    }
}

</style>