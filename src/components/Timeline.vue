<template>
  <div class="container-lg" style="display:inline-block;">
            <div class="justify-content-center mx-2">
            <div class="mx-5" v-for="person in resume">
                     <div class="details">
                      <small class="my-4 period">📅  {{ person.period }}</small>
                <h4>{{ person.name }}</h4>
                 <img :src="person.image" alt="">
                <div class="desc">{{ person.description}}</div>
                     </div>
        </div>
        </div>
        </div>
</template>

<script>
    export default {
        name: 'Timeline',
          data(){
              return{
                  resume:[
                      {
                          name: 'Life Choices Coding Academy',
                          period: ' September 2022 – Present',
                          description: "I am currently learning coding and web development at 'Life Choices Coding Academy' to become a fullstack web developer and learning things that would have taken me ages to learn at rosebank such as HTML, CSS and Bootstrap. Learning at Life Choices has dramatically changed my work ethic for the better.",
                          image: "https://i.postimg.cc/7P5Z66C2/LIFE-CHOICES-ACADEMY-LOGO-ON-BLUE-removebg-preview-1.png"
                      },
                      {
                          name: 'Rosebank College',
                          period: 'January 2022 - August 2022',
                          description: "Studied bachelor's Degree in I.T. at Rosebank College but left due to the fact that I wasn't learning much and when i heard back from life choices i made my decision to leave.",
                          image: "https://i.postimg.cc/XYQ8QQnm/rc-logo.png"
                      },
                      {
                          name: 'Muizenberg High School',
                          period: 'January 2015 - December 2019',
                          description: "I matriculated at Muizenberg High School in 2019 with a bachelor's pass. My subjects were pure Maths, Physics, Business Studies, Music, English, Afrikaans and Life Orientation.",
                          image: "https://i.postimg.cc/CLJkg59f/1940005-1389649074636868-537002596-n.png"
                      }
                  ]
              }
          }
      }
</script>

<style scoped>

.period{
color: orangered;
}

.details{
  margin: 5%;
}

.details small{
  color: rgb(220, 220, 220);
}

.details h4{
  color: red;
}

.details img{
  max-width: 100%;
}

.desc{
  color: rgb(220, 220, 220);
  margin-top: 4%;
}
</style>
 
  
