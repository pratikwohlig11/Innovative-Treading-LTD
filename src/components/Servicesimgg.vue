<template>
  <div class="imgg">
    <div class="container">
      <div class="row py-5">
        <div class="col-6">
          <P>Bathroom we have completed over the years.</P>
        </div>
        <div class="col-6">
          <img
            src="../assets/Images/services2.jpg"
            alt="image loading"
            class="img-fluid"
          />
        </div>
      </div>
      <div class="row py-5">
        <div class="col-6">
          <img
            src="../assets/Images/services3.jpg"
            alt="image loading"
            class="img-fluid"
          />
        </div>
        <div class="col-6">
          <P>Kitchens we have installed over the years.</P>
        </div>
      </div>
      <div class="row py-5">
        <div class="col-6">
          <P
            >Garden Room we have specifically built around each customer’s
            needs.</P
          >
        </div>
        <div class="col-6">
          <img
            src="../assets/Images/services3.jpg"
            alt="image loading"
            class="img-fluid"
          />
        </div>
      </div>
      <div class="row py-5">
        <div class="col-6">
          <img
            src="../assets/Images/services4.jpg"
            alt="image loading"
            class="img-fluid"
          />
        </div>
        <div class="col-6">
          <P>Renovation project we have been involved in. </P>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Servicesimgg",
};
</script>

<style scoped>
.imgg {
  background-color: rgb(195 236 254);
}
.col-6 img {
  height: 105% !important;
  width: 100%;
}
.col-6 p {
  padding: 255px 0px 0px 0px;
  font-weight: bolder;
}
@media only screen and (max-width: 576px){
.col-6{
  height: 50% !important;

}
.col-6 p{
  padding: 30px 0px;
  width: 100%;
}
}
</style>