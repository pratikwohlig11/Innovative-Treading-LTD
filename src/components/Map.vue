<template>
  <div style="background: #c3ecfe">
    <div class="container">
      <div class="where-we-are py-4 px-5">
        <h4 style="color: rgb(233, 69, 94); font-weight: 700">Where We Are</h4>
        <hr />
      </div>

      <div class="map">
        <iframe
          data-v-34b157ca=""
          src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2490.4252103120607!2d-0.08434148436935351!3d51.37686267961394!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x487600cff36bb14b%3A0x432f300759858f54!2sCanning%20Rd%2C%20Croydon%20CR0%206QB%2C%20UK!5e0!3m2!1sen!2sin!4v1635156277135!5m2!1sen!2sin"
          allowfullscreen="allowfullscreen"
          loading="lazy"
          class="size2 map-details"
          style="border: 0px none"
        ></iframe>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.map-details {
  width: 80vw;
  height: 80vh;
  max-width: 100%;
}
</style>
