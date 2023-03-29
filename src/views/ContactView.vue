<template>

<Navbar/>

      <div class="space"></div>
        <div class="contactsec container-lg" id="Contact">
      <h1 class="contact" style="padding-bottom: 6%; color: red;">Contact Me</h1>
      <form action="https://formspree.io/f/xzbwjdvo" method="POST" class="form" style="padding-bottom: 7%;">
          <div class="row">
            <div class="col">
              <input type="text" class="form-control" name="name" placeholder="First name" aria-label="First name" required>
            </div>
            <div class="col">
              <input type="text" class="form-control" name="lastname" placeholder="Last name" aria-label="Last name" required>
            </div>
          </div>
          <div class="mb-3">
            <label for="exampleInputEmail1" class="form-label"></label>
            <input type="email" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp" name="email" placeholder="Your Email" required>
            <div id="emailHelp" class="form-text"></div>
          </div>
        
            <div class="mb-3">
              <label for="exampleFormControlTextarea1" class="form-label"></label>
              <textarea class="form-control" id="exampleFormControlTextarea1" rows="5" name="message" placeholder="Enter Message Here" required></textarea>
            </div>
          
          <button type="submit" class="btn subButton" name="submit">Submit</button>
        </form>

        <div class="deats justify-content-center">
          <text class="mx-5" style="color:red;  font-size: 15px;">Call Me On : +27 83 400 4653</text>
        <text style="color:red; font-size: 15px;">Email : abdulabrahams2002@gmail.com</text>
        </div>
        
    </div>

    <button class="BackNext">
            <router-link to="/projects" @click="scrollTop()"><a>Back</a></router-link>
          </button>
          
<Footer/>          
</template>

<script>
import Navbar from '../components/Navbar.vue'
import Footer from '../components/Footer.vue'
export default{
  name: 'Contact',
  components: {Navbar,Footer},
  
    methods: {
      scrollTop() {
        document.body.scrollTop = document.documentElement.scrollTop = 0;
      }
    }
  }
</script>

<style scoped>
.contactsec{
  min-height: 100vh;
}
.form-control{
    border: 1px solid red;
    background: rgb(26, 26, 26);
    color: red;
}

.subButton{
    font-size: 18px;
    width: 60%;
    border: 1px solid red;
    color: red;
}

.subButton:hover{
  border: 1px solid rgb(189, 16, 16);
  background-color: rgb(189, 16, 16);
  color: white;
}

.contact{
    margin-top: 8%;
    font-size: 34px;
}

.deats{
  display: flex;
}


@media screen and (width <600px){
    .contact{
        margin-top: 20%;
    }

    .contact form{
      margin-top: 10%;
    }

    .deats{
      flex-direction: column;
    }
}
</style>
