<template>
    <div class="photos">
        <div class="image-container">
            <img src="../assets/fabien.png" alt="Fabien">
            <div class="overlay">
                <a href="https://portfolioalexis.alwaysdata.net">
                <p>Bastien<br>
                   Co-Fondateur <br>
                   Développeur Front-End</p></a>
            </div>
        </div>
        <img src="image2.jpg" alt="Alexis">
        <img src="image3.jpg" alt="Lucas">
    </div>
</template>
<style>
    .photos {
        top: 50%;
        text-align: center;
    }
    .photos img {
        margin-top: 10%;
        width: 280px;
        height: auto;
        margin-right: 200px;
    }

.image-container {
  position: relative;
  display: inline-block;
}

.overlay {
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  background-image: linear-gradient(rgba(255, 123, 102, 0), rgba(255, 123, 102, 1));
  overflow: hidden;
  width: 280px;
  height: 0;
  transition: height 0.5s ease-in-out;
}


.overlay p {
  color: white;
  font-size: 18px;
  position: absolute;
  bottom: 0;
  left: 50%;
  transform: translate(-50%, 0);
  margin: 0;
  padding: 10px;
  opacity: 0;
  transition: opacity 0.5s ease-in-out;
}

.image-container:hover .overlay {
  height: 80%;
  width: 280px;
}

.image-container:hover .overlay p {
  opacity: 1;
}


</style>
<script>
export default {
// eslint-disable-next-line vue/multi-word-component-names
  name: 'team_card'
}
</script>