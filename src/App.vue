<template>
  <Navbar />
  <Footer />
</template>

<script>

import Navbar from './components/Navbar.vue'
import Footer from './components/Footer.vue'
export default{
  name: 'App',
  components: {Navbar,Footer},
}
</script>

<style>
 @import url('https://fonts.googleapis.com/css2?family=Orbitron&display=swap');
#app {
  font-family: 'Orbitron', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  font-size: 18px;
}

body{
  background: rgb(12, 12, 12);
}

nav {
  padding: 30px;
}

nav a {
  text-decoration: none;
  font-weight: bold;
  color: #000000;
  align-items: flex-start;
  font-size: 18px;
}

nav a :hover{
  color: #ffffff;
}

nav a.router-link-exact-active {
  color: #ffffff;
}

.BackNext{
  margin-top: 20px;
  border: 2px solid red;
  background: transparent;
}

.BackNext:hover{
  border: 2px solid rgb(189, 16, 16);
  background: rgb(189, 16, 16);
}

.BackNext a{
  padding: 10px;
  text-decoration: none;
  color: red;
}

.BackNext a:hover{
  color: rgb(255, 255, 255);
}
</style>
