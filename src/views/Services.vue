<template>
  <div>
    <Servicesimg/>
    <Servicesbio/>
    <Servicesimgg/>
    <Sfooter />
  </div>
</template>

<script>
import Sfooter from "../components/Sfooter.vue";
import Servicesimg from "@/components/Servicesimg.vue";
import Servicesbio from "@/components/Servicesbio.vue";
import Servicesimgg from "@/components/Servicesimgg.vue";
export default {
  name: "Home",
  components: {
    Sfooter,
    Servicesimg,
    Servicesbio,
    Servicesimgg,
},
};
</script>

<style scoped>
</style>

