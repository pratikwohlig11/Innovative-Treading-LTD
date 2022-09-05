<template>
<div>
    
    <nav class="navbar navbar-expand-lg navbar-light bg-light">
        <div class="container-fluid">
            <a class="nav-link color router-link-exact-active active logo-link" href="/">
              <img src="./assets/Images/logo.svg" class="navbar-brand logo" alt="">
              </a>              
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarSupportedContent">
                <ul class="navbar-nav ms-auto mb-2 mb-lg-0 text-center">
                    
                    <li class="nav-item">
                    <router-link class="nav-link" to="/"
                    >HOME</router-link>
                    </li>

                    <li class="nav-item">
                      <router-link class="nav-link" to="/about"
                    >ABOUT</router-link>
                    </li>

                    <li class="nav-item">
                      <router-link class="nav-link" to="/services"
                    >SERVICES</router-link>
                    </li>

                    <li class="nav-item">
                      <router-link class="nav-link" to="/contact"
                    >CONTACT</router-link>

                    </li>
                   
                </ul>
            </div>
        </div>
    </nav>

    <router-view></router-view>
</div>
</template>

<script>
import Footer from "./components/Footer.vue"  
export default {
components:{
  Footer,
}
}
</script>

<style scoped>
  #app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #111;
}
  .navbar {
  background-color:teal !important;
  box-shadow: 0 15px 10px -15px #111;
  padding: 0px;
  position: fixed !important;
  z-index: 20;
  width: 100%;
}

.nav-link{
  font-weight: bold;
  color: rgba(0, 0, 0, 0.55);
  font-size: 20px;
padding: 4px 10px;
}
.nav-link:focus,
.nav-link:hover {
  color: #eb4760;
}

.nav-items {
  font-family: sans-serif;
}
.logo {
  width: 40%;
  height: 100%;
}
.container-fluid{
  padding: 10px 100px;
}

@media only screen and (max-width: 991px)
{
  .logo-link{
    display: inline-block;
    max-width: 100px;
  }
  .logo{
    width: 175%;
  }
  .container-fluid{
    padding: 3px 10px;
  }
} 

</style>