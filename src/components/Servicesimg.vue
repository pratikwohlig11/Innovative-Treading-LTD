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
  font-size: 35px;
  font-family: Times, serif;
  font-weight: 600;
  position: absolute;
  top: 43%;
  width: 100%;
  text-align: center !important;

}
@media only screen and (max-width: 576px)
{
  .servicep{
    max-width: 100vw !important;
    height: 300px !important;
  }
  .service-img p{
    font-size: 185% !important;
    top: 16% !important;
  }
}
</style>