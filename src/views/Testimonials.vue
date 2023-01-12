<template>
    <div class="space">
        <h1 style="color:red;">Testimonials</h1>
        <Card />
    </div>
</template>

<script>
import Card from '../components/Card.vue'
    export default {
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