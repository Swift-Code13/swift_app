<template>
  <navbar logo="SwiftAndCodeContact.png"/>
  <contact_form></contact_form>
</template>

<script>
// @ is an alias to /src
import contact_form from '@/components/contact-form.vue'
import navbar from "@/components/navbar.vue";
export default {
  name: 'ContactView',
  components: {
    contact_form,
    navbar
  }
}
</script>