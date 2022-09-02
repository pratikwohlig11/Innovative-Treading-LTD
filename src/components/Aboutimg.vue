<template>
  <div>
    <img
      src="../assets/Images/about1.jpg"
      class="aboutp img-fluid"
      alt="image Loading"
    />
    <div class="about-img">
      <p>LEARN ABOUT OUR BUSINESS</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Aboutimg",
};
</script>

<style scoped>

.about-img p {
  color: #53165c !important;
  font-size: 30px !important;
  font-family: Tahoma, Times, serif;
  font-weight: bolder !important;
  position: absolute;
  top: 35%;
  width: 100%;

}
.aboutp {
  opacity: 0.7;
}

@media only screen and (max-width: 991px)
{
  .aboutp{
    width: 100vw;
    height: 300px !important;
  }
  .about-img p{
  font-size: 16px !important;
  top: 20% !important;
}
}

@media only screen and (max-width: 768px)
{
  .about-img p{
  /* font-size: 16px !important; */
  top: 24% !important;
}
}

</style>