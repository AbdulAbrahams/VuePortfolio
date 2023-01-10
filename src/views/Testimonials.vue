<template>
    <div class="space">
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
    margin-top: 8%;
}

@media screen and (width <600px){
    .space{
        margin-top: 20%;
    }
}

</style>