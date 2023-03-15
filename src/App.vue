<template>
  <navbar>
  </navbar>
  <router-view/>
</template>
<style>
  body {
    background-color: black;
  }
</style>
<script>
  import navbar from '@/components/navbar.vue'
  export default {
  name: 'App',
  components: {
    navbar
    }
  }
</script>