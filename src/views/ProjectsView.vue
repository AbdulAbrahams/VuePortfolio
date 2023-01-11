<template>
    <main>
        <h1 style="margin-bottom:4%;margin-top:4%;">Projects</h1>
        <div class="container-lg" style="display:inline-block;">
            <div class="row justify-content-center mx-2">

                <div class="col-sm-9 mx-2" v-for="person in people">
        <div class="card my-3 shadow-sm">
        <img :src="person.image">
        <div class="card-body">
          <p class="card-text" value="Nike">{{ person.name }}</p>
          <div class="d-flex justify-content-between align-items-center">
            <div class="btn-group">
              <a :href="person.netlify"><button type="button" class=" btn btn-danger mx-4 p-2 px-4">Netlify</button></a>
            </div>
            <button class=" btn btn-danger mx-4 my-5 p-2 px-4">GitHub</button>
          </div>
        </div>
      </div>
    </div>

            <!-- <div class="col-sm-4 mx-2" v-for="person in people">
                <div class="project">
                <div class="lines"></div>
                <div class=content>
                    <img :src="person.image">
                <h4>{{ person.name }}</h4>
                <div class="speech">{{ person.testimonials}}</div>
                <div class="buttons my-5">
                    <button class="btn btn-lg btn-outline-danger mx-5 p-2 px-2">Netflify</button>
                    <button class="btn btn-lg btn-outline-danger mx-5 p-2 px-2">Github</button>
                </div>
                   
        </div>
    </div> 
        </div> -->
        </div>
        </div>
        
        
   
    </main>
  
</template>

<script>
    export default {
        name:'Card',
        data(){
            return{
                people:[
                    {
                        name: 'Old Portolio',
                        image: 'https://i.postimg.cc/qv3rdNZJ/land.jpg',
                        netlify: '',
                        github: ''
                    },
                    {
                        name: 'Sneaky Kicks E-commerce Store',
                        image: 'https://i.postimg.cc/vmqHY4dc/Screenshot-2023-01-11-151336.png',
                        netlify: '',
                        github: ''
                    },
                    {
                        name: 'Exclusive Kicks',
                        image: 'https://i.postimg.cc/BnBP95Q3/exclusive.png',
                        netlify: 'https://exclusivekicks.netlify.app/',
                        github: ''
                    },
                    {
                        name: 'First Portfolio',
                        image: 'https://i.postimg.cc/tJc7kD5d/old-portfolio.png',
                        netlify: '',
                        github: ''
                    },
                    {
                        name: 'JavaScript Calculator',
                        image: 'https://i.postimg.cc/QMnLHPxq/Screenshot-2023-01-11-153133.png',
                        netlify: '',
                        github: ''
                    },
                    {
                        name: 'Comic Strip',
                        image: 'https://i.postimg.cc/CLKKtynF/saitama.png',
                        netlify: '',
                        github: ''
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

.card{
    border: 0px;
}

.card img{
    height: 45vh;
}
.card-body{
    background: rgb(26, 26, 26);
}

.card-text{
    color: red;
    font-size: 18px;
    margin-top: 4%;
}
</style>