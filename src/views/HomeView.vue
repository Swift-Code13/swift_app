<template>
  <navbar logo="SwiftAndCode.jpeg" />
  <body>
    <div class="container">
      <h1 class="title">Swift & Code<span class="square"></span></h1>
      <h3>Vite fait, bien fait !</h3>
      <div class="rectangle" id="rectangle1"></div>
      <div class="rectangle" id="rectangle2"></div>
      <div class="rectangle" id="rectangle3"></div>
      <div class="rectangle" id="rectangle4"></div>
      <div class="rectangle pink" id="rectangle5"></div>
      <div class="rectangle blue" id="rectangle6"></div>
    </div>
  </body>
</template>
<style>
body {
  margin: 0;
  padding: 0;
  overflow: hidden;
}
.container {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 100vh;
  width: 100%;
  position: relative;
}
.title {
  font-size: 6rem;
  font-weight: bold;
  color: white;
  text-align: center;
  text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.5);
  z-index: 1;
  display: inline-block;
}
h3 {
  top: 55%;
  margin-top: 10px;
  font-weight: bold;
  color: white;
  position: absolute;
  z-index: 1;
}
.rectangle {
  position: absolute;
  height: 100px;
  width: 100px;
  border-radius: 10px;
  animation: move 4s ease-in-out infinite alternate;
}
#rectangle1 {
  background-color: #62b0f5;
  top: 10%;
  left: 10%;
  animation-delay: 0s;
}
#rectangle2 {
  background-color: #ff9100;
  top: 30%;
  left: 30%;
  animation-delay: 1s;
}
#rectangle3 {
  background-color: #b866ff;
  top: 50%;
  left: 50%;
  animation-delay: 2s;
}
#rectangle4 {
  background-color: #ff7b66;
  top: 70%;
  left: 70%;
  animation-delay: 3s;
}
#rectangle5 {
  background-color: #ff7b66;
  width: 200px;
  top: 0;
  right: -100px;
  animation-delay: 1s;
}
#rectangle6 {
  background-color: #62b0f5;
  width: 200px;
  bottom: 11%;
  left: -100px;
  animation-delay: 1s;
}
.square {
  display: inline-block;
  width: 20px;
  height: 20px;
  background-color: orange;
  margin-left: 5px;
  border-radius: 5px;
}

@keyframes move {
  from {
    transform: translate(0, 0);
  }
  to {
    transform: translate(10px, 10px);
  }
}
.pink {
  animation: move-pink 2s ease-in-out infinite alternate;
}

@keyframes move-pink {
  from {
    transform: translate(0, 0);
  }
  to {
    transform: translate(10px);
  }
}

.blue {
  animation: move-blue 3s ease-in-out infinite alternate;
}

@keyframes move-blue {
  from {
    transform: translate(10px);
  }
}
</style>
<script>
// @ is an alias to /src
import navbar from "@/components/navbar.vue";
export default {
  name: 'HomeView',
  components: {
    navbar
  }
}
</script>