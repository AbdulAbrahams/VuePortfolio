<template>
<h1 class="proHead" style="margin-bottom:4%;margin-top:4%; color:red;">Projects</h1>
    <div class="body">
        <div class="row justify-content-center mx-2">
            <div class="card mx-2 my-3" v-for="content in projects">
        <div class="poster">
            <img :src="content.image" alt="">
        </div>
        <div class="details">
            <h2>{{ content.name }}</h2>
            <div class="buttons">
                <a :href="content.github"><button class="mx-3 p-1">GitHub</button></a>
                <a :href="content.netlify"><button class="mx-3 p-1 px-2">Live</button></a> 
            </div>
        </div>
    </div> 
        </div>
       
    </div>

    <button class="BackNext1">
            <router-link to="/testimonials" @click="scrollTop()"><a>Back</a></router-link>
          </button>
          <button class="BackNext">
            <router-link to="/contact" @click="scrollTop()"><a>Next</a></router-link>
          </button>
    
</template>

<script>
     export default {
        methods: {
      scrollTop() {
        document.body.scrollTop = document.documentElement.scrollTop = 0;
      }
    },
        name:'Card',
        data(){
            return{
                projects:[
                    {
                        name: 'Old Portolio',
                        image: 'https://i.postimg.cc/3J3mdYyG/Screenshot-2023-01-12-134548.png',
                        netlify: 'https://abdulwahhaab.netlify.app/',
                        github: 'https://github.com/AbdulAbrahams/ProjectPortfolio.git'
                    },
                    {
                        name: 'Sneaky Kicks Store',
                        image: 'https://i.postimg.cc/vmqHY4dc/Screenshot-2023-01-11-151336.png',
                        netlify: 'https://sneakykickscpt.netlify.app/',
                        github: 'https://github.com/AbdulAbrahams/JS-project.git'
                    },
                    {
                        name: 'Exclusive Kicks',
                        image: 'https://i.postimg.cc/BnBP95Q3/exclusive.png',
                        netlify: 'https://exclusivekicks.netlify.app/',
                        github: 'https://github.com/AbdulAbrahams/exclusive-kicks.git'
                    },
                    {
                        name: 'First Portfolio',
                        image: 'https://i.postimg.cc/tJc7kD5d/old-portfolio.png',
                        netlify: 'https://abdulabrahams.netlify.app/',
                        github: 'https://github.com/AbdulAbrahams/Portfolio.git'
                    },
                    {
                        name: 'JavaScript Calculator',
                        image: 'https://i.postimg.cc/QMnLHPxq/Screenshot-2023-01-11-153133.png',
                        netlify: 'https://abdulcalculator.netlify.app/',
                        github: 'https://github.com/AbdulAbrahams/calculator.git'
                    },
                    {
                        name: 'Comic Strip',
                        image: 'https://i.postimg.cc/CLKKtynF/saitama.png',
                        netlify: 'https://saitamavsgoku.netlify.app/',
                        github: 'https://github.com/AbdulAbrahams/comic.git'
                    }
                ]
            }
        }
    }
</script>

<style scoped>
.body{
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    overflow-x: hidden;
}

.card{
    background-color: transparent;
    position: relative;
    max-width: 400px;
    height: 350px;
    overflow: hidden;
    border-radius: 10px;
    border: 0px;
}

.card .poster{
    position: relative;
    overflow: hidden;
}

.card .poster::before{
    content: '';
    position: absolute;
    bottom: -100px;
    width: 100%;
    height: 100%;
    background: linear-gradient(0deg,rgb(22, 18, 18) 40%, transparent);
    transition: 0.5s;
    z-index: 1;
}

.card:hover .poster::before{
    bottom: 0px;
}

.card .poster img{
    width: 100%;
    height: 65vh;
    transition: 0.5s;
}

.card:hover .poster img{
    transform: translateY(-50px);
    filter: blur(3px);
}

.card .details{
    position: absolute;
    width: 100%;
    left: 0;
    bottom: 0;
    z-index: 2;
    padding: 20px;
    transition: 0.5s;
}

.card .details .buttons{
    position: absolute;
    width: 100%;
    left: 0;
    bottom: -60px;
    z-index: 2;
    padding: 20px;
    transition: 0.5s;
    background: transparent;
    color: white;

}

.card:hover .details{
    bottom: 50px;
}

.card .details h2{
    color: rgb(252, 20, 20);
    font-size: 31px;
    max-width: 2500px;
}

.card .details .buttons{
    margin-top: 15px;
}

.details .buttons a button{
    background: rgb(201, 19, 19);
    border: 2px solid rgb(201, 19, 19);
    color: rgb(255, 255, 255);
}

.details .buttons a button:hover{
    background: red;
    border: 2px solid red;
    color: rgb(255, 255, 255);
    transition: 0.3s;
}

@media screen and (width <600px){
    .proHead{
        margin-top: 20% !important;
    }
}
</style>
