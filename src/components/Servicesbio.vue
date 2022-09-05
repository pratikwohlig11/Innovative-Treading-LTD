<template>
  <div>
    <div class="container text-center">
      <h2 class="sb py-3"><u>Services Available</u></h2>
      <div class="head py-3 px-4">
        <p>
          With pure dedication to the finest craftsmanship, clients can
          consistently expect a solid commitment to quality, strong work ethic,
          and punctuality. Our personalized options and wide range of prices
          cater to every budget, so you’re sure to find the solutions you need.
        </p>
      </div>
      <div class="taghighlight">
        <b>A Few Highlights</b>
      </div>

      <div class="head-1 py-5 px-4">
        <p class="m-0">
          As a dedicated team of contractors, it gives us great pride to be able
          to call these projects our own. Whatever the size or time commitment
          of each project, our flexibility and strong work ethic allows us to
          carefully plan ahead in order to meet deadlines while delivering high
          quality solutions that are built to last. Take a look at some sample
          projects below.
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Servicesbio",
};
</script>

<style scoped>
.sb {
  color: #e9455e;
}
.container h2 u {
  text-decoration: underline;
  text-decoration-color: teal;
}
.head {
  padding-top: 5%;
  font-family: Courier, Times, serif;
  font-size: 20px;
  color: #212529;
  text-align: start;

  
}
.taghighlight {
  color: #53165c;
  text-align: start;
  font-size: 24px;
  font-family: serif;
  padding: 0px 26px;
}
.head-1 {
  color: #e9455e;
  padding-top: 3%;
  font-family: Courier, Times, serif;
  font-size: 20px;
  text-align: start;
}
@media only screen and (max-width: 576px){
  .head{
    line-height: 25px;
  padding: 5%;
  width: 100%;
  }

  .taghighlight{
    line-height: 0px;
  width: 100%;
  text-align: center;
  }

  .head-1{
  line-height: 24px;
  padding: 7% !important;
  width: 100%;
  }
}
</style>