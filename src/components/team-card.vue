<template>
    <div class="photos">
        <div class="image-container">
            <img src="../assets/fabien.png" alt="Fabien">
            <div class="overlay">
                <a href="https://portfolioalexis.alwaysdata.net">
                <p>Bastien<br>
                   Co-Fondateur <br>
                   CMO <br>
                   Développeur Front-End</p></a>
            </div>
        </div>
        <div class="image-container">
            <img src="../assets/fabien.png" alt="Alexis">
            <div class="overlay">
                <a href="https://portfolioalexis.alwaysdata.net">
                <p>Alexis<br>
                   Co-Fondateur <br>
                   CEO <br>
                   Développeur Fullstack <br>
                   </p></a>
            </div>
        </div>
        <div class="image-container">
            <img src="../assets/fabien.png" alt="Lucas">
            <div class="overlay">
                <a href="https://portfolioalexis.alwaysdata.net">
                <p>Lucas<br>
                   Co-Fondateur <br>
                   CTO <br>
                   Développeur Back-End</p></a>
            </div>
        </div>
    </div>
</template>
<style>
    .photos {
        margin-top: 5%;
        text-align: center;
    }
    .photos img {
        margin-top: 10%;
        width: 280px;
        height: auto;
        border-radius: 5px;
    }

.image-container {
  position: relative;
  display: inline-block;
  width: 280px;
  margin-right: 50px;
  margin-left: 50px;
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
  border-radius: 5px;
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