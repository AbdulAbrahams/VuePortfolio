<template>
    <main class="homeBack">
        <img src="https://i.postimg.cc/V6kJtpmG/d3cc6718eaa8898fba1e612e62511bd9.gif">
        <h4>Web Developer</h4>
        <h1>Abdul Wahhaab Abrahams</h1>
        <button class="learnBtn btn"><router-link to="/about" style="text-decoration: none; color: red;">Learn About Me</router-link></button>
    </main>

</template>

<script>


export default {
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
    color: black;
    background-color: rgb(209, 186, 186);
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