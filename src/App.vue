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
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
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

</style>
