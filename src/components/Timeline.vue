<template>
  <div class="container-lg" style="display:inline-block;">
            <div class="justify-content-center mx-2">
            <div class="" v-for="person in resume">
                     <div class="details my-3">
                      <h6 class="my-4" style="color: orange; margin-bottom: 20px;">📅  {{ person.period }}</h6>
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
                          period: ' September 2022 – March 2023',
                          description: "I learnt coding and web development at 'Life Choices Coding Academy' to become a fullstack web developer and learning things that would have taken me ages to learn at rosebank such as HTML, CSS and Bootstrap. Learning at Life Choices has dramatically changed my work ethic for the better.",
                          image: "https://i.postimg.cc/4ySHrvhV/logo-429x991.png",
                          link: "https://lifechoices.co.za/"
                      },
                      {
                          name: 'Rosebank College',
                          period: 'January 2022 - August 2022',
                          description: "Studied bachelor's Degree in I.T. at Rosebank College but left due to the fact that I wasn't learning much and when i heard back from life choices i made my decision to leave.",
                          image: "https://i.postimg.cc/XvjNkGrb/images.jpg",
                          link: "https://www.rosebankcollege.co.za/"
                      },
                      {
                          name: 'Muizenberg High School',
                          period: 'January 2015 - December 2019',
                          description: "I matriculated at Muizenberg High School in 2019 with a bachelor's pass. My subjects were Pure Mathematics, Physical Sciences, Business Studies, Music, English, Afrikaans and Life Orientation.",
                          image: "https://i.postimg.cc/przy6NRb/Screenshot-2024-05-06-160935.png",
                          link: "https://muizenberghigh.org/"
                      }
                  ]
              }
          }
      }
</script>

<style scoped>

.details{
  margin: 5%;
}

.details small{
  color: rgb(220, 220, 220);
}

.details h4{
  color: red;
}

.details h6{
  font-size: 13px;
}

.details img{
  max-width: 100%;
}

.desc{
  color: rgb(220, 220, 220);
  margin-top: 4%;
}
</style>
 
  
