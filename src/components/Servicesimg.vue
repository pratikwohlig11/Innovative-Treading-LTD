<template>
  <div>
    <img
      src="../assets/Images/services1.jpg"
      class="servicep img-fluid"
      alt="image Loading"
    />
    <div class="service-img">
      <p>OUR SERVICES</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Servicesimg",
};
</script>

<style scoped>
.servicep {
  opacity: 0.6;
}
.service-img p {
  color: #53165c !important;
  font-size: 35px !important;
  font-family: Times, serif;
  font-weight: bolder !important;
  position: absolute;
  top: 42%;
  width: 100%;
}
/* @media only screen and (max-width: 600px)
{
  .servicep{
    width: auto;
    height: 300px !important;
  }
  .service-img{
    width: auto;
    height: auto;
  }
} */
</style>