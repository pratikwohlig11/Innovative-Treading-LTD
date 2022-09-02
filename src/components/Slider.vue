<template>
  <div>
    <div
      id="carouselExampleCaptions"
      class="carousel slide"
      data-bs-ride="carousel"
    >
      <div class="carousel-indicators">
        <button
          type="button"
          data-bs-target="#carouselExampleCaptions"
          data-bs-slide-to="0"
          class="active"
          aria-current="true"
          aria-label="Slide 1"
        ></button>
        <button
          type="button"
          data-bs-target="#carouselExampleCaptions"
          data-bs-slide-to="1"
          aria-label="Slide 2"
        ></button>
        <button
          type="button"
          data-bs-target="#carouselExampleCaptions"
          data-bs-slide-to="2"
          aria-label="Slide 3"
        ></button>
      </div>
      <div class="carousel-inner">
        <div class="carousel-item active">
          <img
            src="../assets/Images/hom1.jpg"
            style="height: 600px; width: 100vw !important"
            class="slider-img d-block w-100"
            alt="Iamge Loading..."
          />
          <div class="carousel-caption d-md-block">
            <p>WELCOME TO INNOVATIVE TRADING LTD.</p>
          </div>
        </div>
        <div class="carousel-item">
          <img
            src="../assets/Images/hom2.jpg"
            style="height: 600px; width: 100vw !important"
            class="slider-img d-block w-100"
            alt="Image Loading..."
          />
          <div class="carousel-caption d-md-block">
            <p>STRONG VALUES AIMED AT EXCEEDING CLIENT NEEDS</p>
          </div>
        </div>
        <div class="carousel-item">
          <img
            src="../assets/Images/hom3.jpg"
            style="height: 600px; width: 100vw !important"
            class="slider-img d-block w-100"
            alt="Image Loading..."
          />
          <div class="carousel-caption d-md-block">
            <p>FLEXIBILITY, STRONG WORK ETHIC & HIGH QUALITY</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Carousel",
};
</script>

<style scoped>
  
.carousel-caption {
  position: absolute;
  top: 50%;
}
.carousel-caption p {
  color: #53165c !important;
  font-size: 27px !important;
  font-family: Tahoma, Times, serif;
  font-weight: bolder !important;
}
.d-block {
  opacity: 0.7;
}
@media only screen and (max-width: 576px)
{
  .slider-img{
    max-width: 100vw !important;
    height: 300px !important;
  }
  .carousel-caption p{
    font-size: 16px !important;
  }
}

</style>