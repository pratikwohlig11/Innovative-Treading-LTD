<template>
  <div>
    <Contactus />
    <ContactData />
    <ContactForm />
    <Map />
    <Cfooter />
  </div>
</template>

<script>
import Contactus from "../components/Contactus.vue";
import ContactData from "@/components/ContactData.vue";
import Map from "@/components/Map.vue";
import ContactForm from "@/components/ContactForm.vue";
import Cfooter from "@/components/Cfooter.vue";
export default {
  name: "Home",
  components: {
    Contactus,
    Map,
    ContactData,
    ContactForm,
    Cfooter,
  },
};
</script>

<style scoped>
</style>

