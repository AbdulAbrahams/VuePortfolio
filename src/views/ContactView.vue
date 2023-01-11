<template>
        <div class="contactsec container-lg" id="Contact">
      <h1 class="contact" style="padding-bottom: 6%; color: red;">Contact Me</h1>
      <form action="https://formspree.io/f/xzbwjdvo" method="POST" class="form" style="padding-bottom: 3%;">
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
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style scoped>

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

.contact{
    margin-top: 8%;
}

@media screen and (width <600px){
    .contact{
        margin-top: 20%;
    }
}
</style>