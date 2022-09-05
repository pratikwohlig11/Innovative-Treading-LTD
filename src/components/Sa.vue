<template>
  <div>
    <div class="sa-data text-center">
      <h2><u>SERVICES AVAILABLE</u></h2>

      <div class="para">
        <p>
          With pure dedication to the finest craftsmanship, clients can
          consistently expect a solid commitment to quality, strong work ethic,
          and punctuality. Our personalized options and wide range of prices
          cater to every budget, so you’re sure to find the solutions you need.
          Take a look below at all of the services that we offer and get in
          touch today.
        </p>
      </div>
     
      <div class="container">
        <div class="images-div row">
         


          <div class="img-pad col-md-6 col-12">
            <figure class="thisimg">
              <img src="../assets/Images/home2.jpg" alt="" class="img-fluid imgdesign">
            </figure>
          </div>

          

          <div class="img-pad col-md-6 col-12">
            <figure class="thisimg">
              <img src="../assets/Images/home3.jpg" alt="" class="img-fluid imgdesign">
            </figure>
          </div>
     
        </div>
      </div>

    </div>
  </div>
</template>

<script>
export default {
  name: "Sa",
};
</script>

<style scoped>
.sa-data {
  font-family: Times, serif;
  background-color: rgb(195 236 254);
  padding: 40px 0px;
}
.para {
  font-family: Times, serif;
  padding: 30px 150px 40px 150px;
  text-align: start;
  font-size: 20px;
  font-weight: 600;
}
.imgdesign{
  border: 2px solid #fff;
  box-shadow: rgba(0, 0, 0, 0.64) 0px 0px 26px 8px;
 
  
}
.h2 {
  font-family: Times, serif;
  font-weight: 600;
}
@media only screen and (max-width: 576px) {
  .sa-data h2 u {
    font-size: 26px;
    line-height: 25px;
    font-weight: 600;
  }
  .para {
    padding: 7%;
  }
  .para p {
    font-size: 18px;
  }
  .padd-pic{
    padding: 2% 15%;

  }
  .img-pad{
    padding: 5% 10%;  
  }
}

</style>