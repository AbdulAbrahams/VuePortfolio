<template>
    <section id="experience" class="body2 container">
      <h3 style="text-align: center;margin-top: 2rem;text-shadow: 0.5px 0.5px black;">Education & Experience</h3>
      <ul class="timeline" style="margin-top: 2rem;text-shadow: 0.2px 0.5px rgb(0, 0, 0);margin-left: 0.5rem;margin-right: 0.5;">
      <li class="timeline" v-for="details in resume">
          <div class="timeline-panel">
            <div class="lines"></div>
            <div class="timeline-heading">
                <img :src="details.image" style="max-width:100%; max-height:100%; position: relative;">
                <p class="timeline-period">
                <small style="color: orange;"><i class="fa fa-calendar"></i> {{ details.period }}</small>
              </p>
              <h4 class="timeline-title" style="color: red;">{{ details.name }}</h4>
            </div>
            <div class="timeline-body">
              <p style="margin-top:8%; margin-bottom: 8%; color: white;"> {{ details.description }} </p>
            </div>>
          </div>
        </li>

        <li class="timeline-inverted" v-for="details in resumeRight">
          <div class="timeline-panel">
            <div class="lines"></div>
            <div class="timeline-heading">
                <img :src="details.image" style="max-width:100%; max-height:100%; position: relative;">
                <p class="timeline-period">
                <small style="color: orange;"><i class="fa fa-calendar"></i> {{ details.period }}</small>
              </p>
              <h4 class="timeline-title" style="color: red;">{{ details.name }}</h4>
            </div>
            <div class="timeline-body">
              <p style="margin-top:8%; margin-bottom: 8%; color: white;"> {{ details.description }} </p>
            </div>>
          </div>
        </li>
      </ul>
    </section>
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
                      }
                  ],

                  resumeRight:[
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

/* .timeline{
    margin-top: 20%;
    position: relative;
    min-width: 300px;
    max-width: 400px;
    height: 450px;
    background: black;
    color: orangered;
} */

.timeline .lines{
position: absolute;
inset: 0;
background: black;
overflow: hidden;
}

.timeline .lines::before{
    content: '';
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    width: 900px;
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

.timeline .lines::after{
    content: '';
    position: absolute;
    inset: 4px;
    background: rgb(26, 26, 26);
}
  .timeline {
    list-style: none;
    padding: 20px 0 20px;
    position: relative;
    color: black;
  }
  .timeline:before {
    top: 0;
    bottom: 0;
    position: absolute;
    content: " ";
    width: 8px;
    background-color: #ff0000;
    left: 50%;
    margin-left: -3.5px;
  }
  .timeline > li {
    margin-bottom: 20px;
    position: relative;
  }
  .timeline > li:before,
  .timeline > li:after {
    display: table;
  }
  .timeline > li:after {
    clear: both;
  }
  .timeline > li:before,
  .timeline > li:after {
    content: " ";
    display: table;
  }
  .timeline > li:after {
    clear: both;
  }
  .timeline > li > .timeline-panel {
    width: 46%;
    float: left;
    border: 1px solid #ff000000;
    border-radius: 2px;
    background-color: rgba(248, 242, 242, 0);
    padding: 20px;
    position: relative;
    -webkit-box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.175);
    box-shadow: 0 1px 6px rgba(0, 0, 0, 0.175);
  }


  .timeline > li.timeline-inverted > .timeline-panel {
    float: right;
  }
  .timeline > li.timeline-inverted > .timeline-panel:before {
    border-left-width: 0;
    border-right-width: 15px;
    left: -15px;
    right: auto;
  }
  .timeline > li.timeline-inverted > .timeline-panel:after {
    border-left-width: 0;
    border-right-width: 14px;
    left: -14px;
    right: auto;
  }
 
  .timeline-title {
    position: absolute;
    /* margin-bottom: 3%; */
    color: black;
  }
  .timeline-body > p, .timeline-body > ul {
    position: relative;
    margin-bottom: 0;
  }
  .timeline-body > p + p {
    position: relative;
    margin-top: 8;
  }

  .timeline-period{
    position: relative;
    margin-top: 5%;
  }

  .timeline-body img{
    position: absolute;
  }
  </style>
 
  