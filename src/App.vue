<template>
  <div id="app">
    <div class="navigation-bar">
      <nav class="navbar navbar-expand-lg bg-light stikc">
        <div class="container">
          <!-- my class start -->
          <div class="myclass">
            <!-- logo start -->
            <a class="navbar-brand text-start" href="#">
              <a
                class="nav-link color router-link-exact-active active"
                href="/"
              >
                <img
                  src="./assets/Images/logo.svg"
                  alt="Images Loading"
                  class="img-fluid logo"
                />
              </a>
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
            <div
              class="navv content collapse navbar-collapse"
              id="navbarSupportedContent"
            >
              <ul class="navbar-nav me-auto mb-2 mb-lg-0">
                <li class="home1 nav-item">
                  <router-link class="nav-link" to="/">HOME</router-link>
                </li>

                <li class="home2 nav-item">
                  <router-link class="nav-link" to="/about">ABOUT </router-link>
                </li>

                <li class="home3 nav-item">
                  <router-link class="nav-link" to="/services"
                    >SERVICES</router-link
                  >
                </li>

                <li class="home4 nav-item">
                  <router-link class="nav-link" to="/contact"
                    >CONTACT</router-link
                  >
                </li>
              </ul>
            </div>
            <!-- Links End -->
          </div>
          <!-- my class end -->
        </div>
      </nav>
    </div>
    <router-view></router-view>
  </div>
</template>

<script>
import Footer from "./components/Footer.vue";

export default {
  components: {
    Footer,
  },
};
</script>

<style scoped>
.myclass {
  display: flex;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #111;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: black;
}

.nav-link:focus,
.nav-link:hover {
  color: #eb4760;
}

.nav-items {
  font-family: sans-serif;
}
.logo {
  width: 50%;
  height: 100%;
}

.navbar {
  background-color:teal !important;
  box-shadow: 0 15px 10px -15px #111;
  /* transition: s; */
  padding: 0px;
  position: fixed !important;
  z-index: 20;
  width: 100%;
}

.nav-link {
  color: rgba(0, 0, 0, 0.55);
  font-size: 20px;
  font-weight: 900;
  padding: 10px;
}
.nav-link:hover {
  color: #eb4760;
}
.content {
  padding: 0px 0px 8px 0px;
}
.home1 {
  margin: 0 8px;
}
.home2 {
  margin: 0 8px;
}
.home3 {
  margin3: 0 8px;
}
.home4 {
  margin: 0 8px;
}
.navv {
  margin: 0px -60px 0px 0px;
}

</style>
