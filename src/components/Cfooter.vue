<template>
  <div>
    <footer class="footer pt-5 pb-4">
      <div class="container text-center text-md-left">
        <div class="row text-center text-md-left">
          <!-- links starts -->
          <div class="box col-sm-12 col-md-5">
            <div class="fimage">
              <a
                class="nav-link color router-link-exact-active active"
                href="/"
              >
                <img
                  src="../assets/Images/logo.svg"
                  alt="image loading"
                  class="imgggg img-fluid"
                />
              </a>
            </div>
            <br />
            <div>
              <ul class="list">
                <li><a href="/" class="nav-link">Home</a></li>
                <br />
                <li><a href="/about" class="nav-link">About</a></li>
                <br />
                <li><a href="/services" class="nav-link">Services</a></li>
                <br />
              </ul>
            </div>
          </div>
        </div>
      </div>
    </footer>
  </div>
</template>

<script>
export default {
  name: "Cfooter",
};
</script>

<style scoped>
.footer {
  background-color: teal;
  line-height: 28px;
  font-size: 18px;
  padding-top: 2% !important;
  padding-bottom: 2% !important;
  box-sizing: border-box;
}
.box {
  margin: 0 auto;
}
.list {
  list-style-type: none;
  font-size: 140%;
  color: #53165c !important;
  font-weight: 550px;
}
.nav-link:focus,
.nav-link:hover {
  color: #eb4760 !important;
}
</style>