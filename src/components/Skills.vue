<template>
      <div class="container-lg" style="display:inline-block;">
            <div class="row justify-content-center mx-2">
            <div class="col-sm-4 mx-2 my-2 bg-dark skillsCol" v-for="pic in skills">
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
                        image: 'https://i.postimg.cc/76DKxRLK/pngegg-5.png'
                    },
                    {
                        image: 'https://i.postimg.cc/G2yjQ2YH/html-png.png'
                    },
                    {
                        image: 'https://i.postimg.cc/gcKhP8YG/bootstrap.png'
                    },
                    {
                        image: 'https://i.postimg.cc/152h991M/pngegg-7.png'
                    },
                    {
                        image: 'https://i.postimg.cc/QMSTTYb4/pngegg-6.png'
                    },
                    {
                        image: 'https://i.postimg.cc/CxMw1XgR/pngegg-2.png'
                    },
                    {
                        image: 'https://i.postimg.cc/Zn6MFbrJ/pngegg-1.png'
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
    margin: 5%;
    max-width: 100%;
    max-height: 80%;
}

.skillsCol:hover{
    opacity: 50%;
}
</style>
