<template>
  <div class="text-center footer-contact-us">
    <div class="content">
      <ContactForm />
      <SocialIcons />
    </div>
  </div>
</template>

<script>
import ContactForm from "@/components/ContactForm";
import SocialIcons from "@/components/SocialIcons";
export default {
  name: "ContactUs",
  components: {
    ContactForm,
    SocialIcons
  }
}
</script>

<style scoped>

</style>
