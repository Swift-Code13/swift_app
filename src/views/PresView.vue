<template>
  <navbar logo="SwiftAndCode.jpeg"/>
  <presCard></presCard>
</template>
<style>
  body{
    overflow-x: hidden;
    overflow-y: auto;
  }
</style>
<script>
import navbar from "@/components/navbar.vue";
import presCard from "@/components/pres-card.vue";
// @ is an alias to /src
export default {
  name: 'PresView',
  components: {
    navbar,
    presCard
  }
}
</script>