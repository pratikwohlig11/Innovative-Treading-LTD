<template>
  <div>
    <Servicesimg/>
    <Servicesbio/>
    <Servicesimgg/>
    <Footer />
  </div>
</template>

<script>
import Footer from "../components/Footer.vue";
import Servicesimg from "@/components/Servicesimg.vue";
import Servicesbio from "@/components/Servicesbio.vue";
import Servicesimgg from "@/components/Servicesimgg.vue";
export default {
  name: "Home",
  components: {
    Footer,
    Servicesimg,
    Servicesbio,
    Servicesimgg,
},
};
</script>

<style scoped>
</style>

