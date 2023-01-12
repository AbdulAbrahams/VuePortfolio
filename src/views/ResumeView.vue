<template>
    <div class="resume">
    <h1>Resume</h1>
    <Timeline />
    <h1>Skills</h1>
    <Skills /> 
    </div>
 
</template>

<script>
import Timeline from '../components/Timeline.vue'
import Skills from '../components/Skills.vue'
    export default {
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
</style>