<template>
    <footer class="d-flex justify-content-between align-items-center py-3 my-5 container-lg">
          <div class="col-md-4 mx-5 d-flex align-items-center">
            <a href="#" class="mb-3 me-2 mb-md-0 text-muted text-decoration-none lh-1">
              <span class="text-muted"><img src="https://i.postimg.cc/66dv9ZGS/wahhaab-web-development-high-resolution-logo-color-on-transparent-background.png" width="70px" height="40px"></span>
            </a>
            
          </div>
      
          <div class="footer-bar mx-5">
            <a href="https://www.instagram.com/abdul_abrahams_/"><i class="fa fa-instagram"></i></a> 
            <a href="https://www.linkedin.com/in/abdul-wahhaab-abrahams-506142222/"><i class="fa fa-linkedin"></i></a> 
            <a href="https://github.com/AbdulAbrahams"><i class="fa fa-github"></i></a>
          </div>
        </footer>
</template>

<script>
    export default {
        name: 'Footer',
    }
</script>

<style scoped>

footer{
  border-top: 2px solid red;
}
.footer-bar{
    font-size: 25px;
}
.footer-bar a{
    margin: 3px;
}

.footer-bar a i{
    color: rgb(255, 0, 0) !important;
}
</style>