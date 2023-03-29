<template>

<router-view/>

</template>

<script>

export default{
  name: 'App',
}
</script>

<style>
 @import url('https://fonts.googleapis.com/css2?family=Orbitron&display=swap');
 
 *{
  font-family: 'Orbitron', sans-serif;
 }
#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  font-size: 18px;
}

.space{
    margin-top: 80px;
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

.BackNext1{
  margin-top: 20px;
  border-right: 0px !important;
  border: 2px solid red;
  background: transparent;
}

.BackNext{
  margin-top: 20px;
  border: 2px solid red;
  background: transparent;
}

.BackNext1:hover{
  border: 2px solid rgb(189, 16, 16);
  background: rgb(189, 16, 16);
}

.BackNext1 a{
  padding: 10px;
  text-decoration: none;
  color: red;
}

.BackNext1 a:hover{
  color: rgb(255, 255, 255);
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
