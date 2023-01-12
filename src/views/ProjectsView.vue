<template>
    <main>
        <h1 style="margin-bottom:4%;margin-top:4%; color:red;">Projects</h1>
    <div class="container-lg" style="display:inline-block;">
            <div class="row justify-content-center mx-2">
            <div class="col-sm-4 mx-2 my-2 bg-dark skillsCol" v-for="pic in projects">
                     <p class="card-text my-2">{{ pic.name }}</p> 
                     <img :src="pic.image" alt="">
                      <a :href="pic.github"><button class="proBut btn mx-4 p-2 px-4">GitHub</button></a>
                      <a :href="pic.netlify"><button class="proBut btn mx-4 p-2 px-4">Live</button></a>
        </div>
        </div>
    </div>
    </main>
  
</template>

<script>
    export default {
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
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

main{
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    overflow-x: hidden;
}
.skillsCol{
    height: 35vh;
    max-width: 350px;
}

.skillsCol img{
    margin: 3%;
    max-width: 80%;
    max-height: 50%;
}

.skillsCol img:hover{
    opacity: 30%;
}

.card-text{
    color: red;
}

.proBut{
    color: rgb(255, 255, 255);
    background-color: rgb(223, 21, 21);
}
.proBut:hover{
    background-color: rgb(197, 56, 56);
}
</style>