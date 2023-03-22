<template>
  <router-view/>
  <div class="footer">
      <p>Copyright © Swift&Code</p>
    </div>
</template>
<style>
@import url('https://fonts.googleapis.com/css2?family=Lilita+One&display=swap');
  body {
    background-color: black;
    font-family: 'segoe-ui-semibold-regular', sans-serif;
    overflow: hidden;
  }
  .footer {
    position:relative;
    bottom: 0;
    color: #fff;
  }
</style>
<script>
  export default {
  name: 'App',
  }
</script>