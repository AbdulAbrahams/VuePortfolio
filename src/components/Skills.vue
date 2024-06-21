<template>
      <div class="container-lg" style="display:inline-block;">
            <div class="row justify-content-center mx-2">
            <div class="col-md-3 mx-2 my-2 bg-dark skillsCol" v-for="pic in skills">
                      <img :src="pic.image" alt="">
        </div>
        </div>
        </div>
</template>

<script>
    export default {
        name: 'Skills',
        data(){
              return{
                  skills:[
                    {
                        image: 'https://i.postimg.cc/kgnXtM8B/HTML3.png'
                    },
                    {
                        image: 'https://i.postimg.cc/0QZ848Jw/css.png'
                    },
                    {
                        image: 'https://i.postimg.cc/W3cGMJ7M/bootstrap.png'
                    },
                    {
                        image: 'https://i.postimg.cc/TYsWVDdp/JS.png'
                    },
                    {
                        image: 'https://i.postimg.cc/76P68HHF/Vue.png'
                    },
                    {
                        image: 'https://i.postimg.cc/43YGzY3N/MySQL.png'
                    },
                    {
                        image: 'https://i.postimg.cc/K8KpfBtV/Node.png'
                    },
                    {
                        image: 'https://i.postimg.cc/x1bgMY2V/Wordpress.png'
                    },
                    {
                        image: 'https://i.postimg.cc/ZYpfDpsv/Java.png'
                    },
                    {
                        image: 'https://i.postimg.cc/Hsjt1MBt/sel-3.png'
                    }
                  ]
             }
        }
    }
</script>

<style scoped>
.skillsCol{
    height: 20vh;
}

.skillsCol img{
    margin-top: 5%;
    max-width: 100%;
    max-height: 80%;
}

.skillsCol:hover{
    opacity: 50%;
}

@media screen and (width < 768px) {
.skillsCol img{
    margin-top: 2% !important;
}
}

@media screen and (width < 425px) {
.skillsCol img{
    margin-top: 5% !important;
}
}
</style>
