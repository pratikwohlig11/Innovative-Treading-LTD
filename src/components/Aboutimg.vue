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
/*  
  position: absolute;
  top: 50%; 
  width: 100%; */
.about-img p {
  color: #53165c !important;
  font-size: 30px !important;
  font-family: Tahoma, Times, serif;
  font-weight: bolder !important;
  position: absolute;
  top: 50%;
  width: 100%;
}
.aboutp {
  opacity: 0.7;
}
</style>