<template>
<Navbar/>
<div class="space"></div>
  <section class="aboutsec container-lg"  id="About">
    <div class="me">
      <div class="myLines"></div>
      <img src="https://iili.io/dH1bC8X.png" class="aboutpic">
    </div>
      
      <div>
      <h2>About Abdul Wahhaab</h2>
      <p>Hi! I am Abdul Wahhaab Abrahams, but you can call me Wahhaab. I'm an aspiring fullstack Web Developer that enjoys helping out wherever I can and sharing the knowledge that i've gained as well as take in new information and learn more. I'm a bit of a perfectionist at times and try to recreate things exactly as I envisioned it, but i see that as a strength and not a weakness.</p>
      <p>When I am not in front of the computer coding, I spend my time playing basketball🏀 working out at the gym🏋️‍♂️playing games with my friends🎮and spending time with my family👪.</p>
    </div>
  </section>

          <button class="BackNext1">
            <router-link to="/" @click="scrollTop()"><a>Back</a></router-link>
          </button>
          <button class="BackNext">
            <router-link to="/resume" @click="scrollTop()"><a>Next</a></router-link>
          </button>
          
<Footer/>          
</template>

<script>
  
import Navbar from '../components/Navbar.vue'
import Footer from '../components/Footer.vue'

export default{
  name: 'About',
  components: {Navbar,Footer},
  
    methods: {
      scrollTop() {
        document.body.scrollTop = document.documentElement.scrollTop = 0;
      }
    }
  }
</script>

<style scoped>
        .aboutsec{
            display: flex;
            justify-content: flex-start;
            align-items: center;
            width: 100%;
            margin-top: 11%;
            margin-bottom: 8%;
          }
  
        .aboutpic{
          position: relative;
          top: 6px;
          width: calc(95.3%);
          height: calc(97%);
        }

        .me{
    position: relative;
    min-width: 300px;
    width: 1200px;
    height: 450px;
    background: black;
    color: orangered;
    /* margin-top: 8%; */
    /* transition: 0.5s; */
}

.me .myLines{
position: absolute;
inset: 0;
background: black;
overflow: hidden;

}

.me .myLines::before{
    content: '';
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    width: 600px;
    height: 120px;
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
.me .myLines::after{
    content: '';
    position: absolute;
    inset: 7px;
    background: rgb(26, 26, 26);
}
        .aboutsec h2{
            color: #ff0000;
            font-weight: 900;
            font-size: 6vh;
            /* margin-top: 8%; */
            left: 0;
            line-height: 5rem;
          }
          .aboutsec p{
            color: rgb(220, 220, 220);
            padding-left: 8%;
          }

          @media screen and (width <= 768px) {
              body{
                overflow-x: hidden !important;
              }

              .me{
                max-width: 300px;
              }

            .aboutsec{
              flex-direction: column;
              overflow-x: hidden;
            }
            .aboutpic{
              position: relative;
              top: 6px;
              max-width: calc(97%);
              max-height: calc(97.8%);
            }

            .aboutsec p{
              padding-left: 0;
            }
          }

          @media screen and (width <600px){
    .aboutsec{
        margin-top: 20%;
    }
}
</style>


