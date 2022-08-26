<template>
  <div>
    <div class="contactimg">
      <img
        src="../assets/Images/contact1.jpg"
        class="img-fluid"
        alt="image Loading"
      />
    </div>
    <div class="contact-img">
      <p>CONTACT US</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Contactus",
};
</script>

<style scoped>
.contact-img {
  position: absolute;
  top: 50%; 
  width: 100%;
}
.contact-img p {
  color: #53165c !important;
  font-size: 45px !important;
  font-family: Tahoma, Times, serif;
  font-weight: bolder !important;
  margin-top: 60px;
}

.contactimg {
  opacity: 0.7;
}
.words {
  background-color: skyblue;
  color: rgb(233, 69, 94);
  font-size: 26px !important;
  /* text-align: center; */
  padding: 50px 130px 0 130px;
}
.mark {
  background-color: skyblue;
}
</style>