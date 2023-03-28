<template>
        <div class="container">
        <div class="row">
        <div class="col-md-4 peeps" v-for="person in people">
        <div class="person">
        <div class="lines"></div>
                    <div class="cardImage">
                        <img :src="person.image">
                     </div>
                <div class=content>
                     <div class="details">
                <h4>{{ person.name }}</h4>
                <h5 style="color: orange;">Web Developer</h5>
                <div class="speech mx-1">{{ person.testimonials}}</div>
                    </div>
               </div>
        </div>
        </div>
        </div>
        </div>
  
</template>

<script>
    export default {
        name:'Card',
        data(){
            return{
                people:[
                    {
                        name: "Jia Daniels",
                        testimonials: "Abdul is a very productive and efficient person. He takes pride in his work and works very well in teams as well as alone. He is trustworthy and loyal and would be a great addition to any company.",
                        image: "https://i.postimg.cc/rmGy1V8y/IMG-9927.jpg",
                    },
                    {
                        name: "Savannah Samuels",
                        testimonials: "Abdul always strives to learn new things to help him in the future and his always available to help and teach other individuals. Always looks on the bright side of things and is always positive in any situation.",
                        image: "https://i.postimg.cc/9MBV4Lpr/IMG-20220904-134609-306.jpg",
                    },
                    {
                        name: "Abdul Azeez Kemp",
                        testimonials: "An absolute great guy, hard worker and a goal driven personality. Always takes on the next challenge that comes to him and knows how to communicate and socialise in his surroundings.",
                        image: "https://i.postimg.cc/T3W6jd08/Screenshot-20221101-100639-edit-159098746871600.jpg",
                    },
                    {
                        name: "Aneeqa Brown",
                        testimonials: "Abdul Wahhaab is a highly thought intellectual. His hardworking, creative but ambitious to recreate his vision exactly. He always provide a helping hand. He has great communication and leadership skills that a company needs.",
                        image: "https://i.postimg.cc/nzFgWp4h/1667550652724.jpg",
                    },
                    {
                        name: "Jake Jansen",
                        testimonials: "Abdul is a very creative and dedicated person with what he does. Works well in teams and is a pro-active worker. Great communication skills and open to ideas of others. He is also very driven to be the best of his caliber.",
                        image: "https://i.postimg.cc/65vjYykh/me.jpg",
                    },
                    {
                        name: "Mu'eed Brown",
                        testimonials: "Abdul is a very ambitious person who is not afraid to work towards achieving his goals. He is also very creative with his work. He is one of the most creative developers around. Abdul won't be afraid to assist those in need.",
                        image: "https://i.postimg.cc/XvVsjxp2/my-image.jpg",
                    }
                ]
            }
        }
    }
</script>

<style scoped>

.row{
justify-content: center;
}

.prac{
background: red;
height: 100px;
width: 100px;
}

.peeps{
  justify-content: center !important;
  width: 450px;
}

.container{
    overflow-x: hidden;
}

.person{
    margin-top: 20%;
    position: relative;
    min-width: 300px;
    height: 520px;
    background: black;
    color: orangered;
    /* transition: 0.5s; */
}

.person .lines{
position: absolute;
inset: 0;
background: black;
overflow: hidden;
}

.person .lines::before{
    content: '';
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    width: 700px;
    height: 200px;
    background: linear-gradient(transparent, rgb(255, 0, 0), rgb(255, 0, 0), transparent);
    animation: animate 8s linear infinite;
}

@keyframes animate{
    0%{
        transform: translate(-50%, -50%) rotate(0deg);
    }
    100%{
        transform: translate(-50%, -50%) rotate(360deg);
    }
}

.person .lines::after{
    content: '';
    position: absolute;
    inset: 4px;
    background: rgb(26, 26, 26);
}

.person .cardImage{
    position: absolute;
    top: -50px;
    left: 50%;
    transform: translateX(-50%);
    width: 250px;
    height: 250px;
    background-color: black;
    transition: 0.5s;
    z-index: 10;
    overflow: hidden;
}

.person .cardImage::before{
    content: '';
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    width: 600px;
    height: 120px;
    background: linear-gradient(transparent, rgb(255, 0, 0), rgb(255, 0, 0), transparent);
    animation: animateAnti 6s linear infinite;
}

@keyframes animateAnti{
    0%{
        transform: translate(-50%, -50%) rotate(0deg);
    }
    100%{
        transform: translate(-50%, -50%) rotate(-360deg);
    }
}

.person .cardImage::after{
    content: '';
    position: absolute;
    inset: 4px;
    background: rgb(26, 26, 26);
}

.person .cardImage img{
    position: absolute;
    top: 5px;
    left: 5px;
    z-index: 1;
    width: calc(96.5%);
    height: calc(96.5%);

}

.person .content{
    padding: 10px;
    position: absolute;
    width: 100%;
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    overflow: hidden;
}

.person .content h4{
margin-top: 190px;
color: rgb(255, 0, 0);
}

.card .content .details{
    padding: 3%;
    /* font-size: 1.25em; */
}

.speech{
    margin-top: 3%;
    color: rgb(220, 220, 220);
}

@media screen and (width 420px <= 770px) {
  .peeps{
  justify-content:center !important;
}
}

@media screen and (width <= 375px) {
  .peeps{
  min-width: 300px;
}
}
</style>
