<template>
  <div id="right">
    <div id="form">
      <div id="titre">
        <br><center><h1>CONTACTEZ-NOUS</h1></center><br>
      </div>
      <form method="post" action="process.php">
        <div id="input-group">
          <input type="text" id="name" name="name" required>
          <label for="name"><i class="fa-sharp fa-solid fa-user"></i> Votre nom</label>
        </div>
        <div id="input-group">
          <input type="email" id="email" name="email" required>
          <label for="email"><i class="fa-solid fa-at"></i> Votre email</label>
        </div>
        <div id="input-group">
          <input type="text" id="subject" name="subject" required>
          <label for="subject"><i class="fa-solid fa-envelope"></i> Votre Sujet</label>
        </div>
        <div id="input-group">
          <textarea id="message" name="message" rows="5" required></textarea>
          <label for="message"><i class="fa-solid fa-comments"></i> Votre Message</label>
        </div>

        <center><input type="submit" value="Envoyer"></center>
      </form>
    </div>
  </div>
  <div id="center"><span id="color"></span></div>
  <div id="left">
    <h1>EMPLACEMENT</h1>
    <p><i class="fa-solid fa-location-dot"></i> Marseille</p>
    <h1>SUIVEZ-NOUS</h1>
    <i class="fa-brands fa-instagram"></i>
    <i class="fa-brands fa-facebook"></i>
    <i class="fa-brands fa-twitter"></i>
    <i class="fa-brands fa-linkedin"></i>
  </div>
</template>
<style>
      body {
        font-family: Arial, sans-serif;
      }
      h1{
        color: white;
      }
      form {
        max-width: 600px;
        width: 90%;
      }
      input,
      textarea {
        width: 100%;
        padding: 10px;
        outline: 0;
        background-color: white;
        box-sizing: border-box;
        margin-bottom: 10px;
        border-radius: 20px;
      }
      input[type="submit"] {
        background-color: transparent;
        color: white;
        width: 30%;
        border: 2px solid white;
        cursor: pointer;
        transition: 0.7s;
        border-radius: 5px;
      }
      input[type="submit"]:hover {
        background-color: #62B0F5;
        transition: 0.7s;
      }
      #form {
        padding: 30px;
      }
      label {
        color: gray;
        position: absolute;
        margin-bottom: 30px;
        left: 5px;
        top: 0;
        padding: 10px;
        transition: 0.2s;
      }
      #input-group {
        margin-bottom: 30px;
        position: relative;
      }
      input:focus~label, input:valid~label, textarea:focus~label, textarea:valid~label {
        top: -35px;
        font-size: 14px;
      }
      #titre {
        width: 85%;
        margin-bottom: 10px;
        border-radius: 30px;
        font-family: 'Oswald', sans-serif;
      }
      #right {
        margin-left: 60%;
      }
      #center {
        width: 300px;
        height: 0;
        position: absolute;
        top: 50%;
        left: 53%;
        transform: translate(-50%, -50%);
        background: #62B0F5;
        animation: anim 1s linear forwards;
      }
      #left {
        position: absolute;
        top: 15%;
        left: 14%;
      }
      #left h1 {
        font-family: 'Oswald', sans-serif;
        margin-bottom: 20px;
      }
      #left i {
        font-size: 30px;
        margin-left: 15px;
        color: white;
      }
      #left p {
        color: gray;
        font-family: 'Oswald', sans-serif;
        font-size: 25px;
      }
      @keyframes anim {
        100%{
          height: 100%;
        }
      }
    </style>
<script>
export default {
// eslint-disable-next-line vue/multi-word-component-names
  name: 'contact_form'
}
</script>