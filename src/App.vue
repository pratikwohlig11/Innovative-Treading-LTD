<template>
  <div id="app">
    <div class="container">
      <nav class="navbar navbar-expand-lg bg-light">
        <div class="container">
          <!-- my class start -->
          <div class="myclass">
            <!-- logo start -->
            <a class="navbar-brand text-start" href="#">
              <img
                src="./assets/Images/logo.svg"
                alt="Images Loading"
                class="img-fluid logo"
              />
            </a>
            <!-- logo end -->

            <!-- respo btn  start -->
            <div class="respo-btn">
              <button
                class="navbar-toggler"
                type="button"
                data-bs-toggle="collapse"
                data-bs-target="#navbarSupportedContent"
                aria-controls="navbarSupportedContent"
                aria-expanded="false"
                aria-label="Toggle navigation"
              >
                <span class="navbar-toggler-icon"></span>
              </button>
            </div>
            <!-- respo btn  end -->


            <!-- Links Start -->
          <div class="collapse navbar-collapse" id="navbarSupportedContent">
            <ul class="navbar-nav me-auto mb-2 mb-lg-0">
              <li class="nav-item">
                <a class="nav-link" href="#">HOME</a>
              </li>

              <li class="nav-item">
                <a class="nav-link" href="#">ABOUT </a>
              </li>

              <li class="nav-item">
                <a class="nav-link" href="#">SERVICES</a>
              </li>

              <li class="nav-item">
                <a class="nav-link" href="#">CONTACTS</a>
              </li>
              <li class="nav-item">
                <a class="nav-link disabled"></a>
              </li>
            </ul>
          </div>
          <!-- Links End -->

          </div>
          <!-- my class end -->

          
        </div>
      </nav>
    </div>
  </div>
</template>

<script>
import Home from "../src/views/Home.vue";

export default {
  components: {
    Home,
  },
};
</script>

<style>
.myclass{
  display: flex;

}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}

.nav-items {
  font-family: sans-serif;
}
.logo {
  width: 30% !important;
  height: 100%;
}
</style>
