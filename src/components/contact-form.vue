<template>
  <div id="form">
    <div id="titre">
      <br><center><h1>Contactez-Nous</h1></center><br>
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
</template>
<style>
      body {
        font-family: Arial, sans-serif;
      }
      h1{
        color: white;
      }
      form {
        max-width: 400px;
        margin: 0 auto;
      }
      input,
      textarea {
        width: 100%;
        padding: 10px;
        box-sizing: border-box;
        margin-bottom: 10px;
        resize: vertical;
        border-radius: 20px;
        color: white;
      }
      input[type="text"], input[type="email"], textarea{
        background-color: #62B0F5;
      }

      input::placeholder, textarea::placeholder {
        color: #989797;
      }
      input[type="submit"] {
        background-color: #62B0F5;
        color: white;
        padding: 10px 20px;
        border: none;
        cursor: pointer;
        border-radius: 20px;
        transition: 0.7s;
      }
      input[type="submit"]:hover {
        background-color: #114371;
        transition: 0.7s;
        padding: 20px;
      }
      #form {
        border: 4px solid #62B0F5;
        width: 30%;
        padding: 30px;
        margin: 5% auto auto;
        border-radius: 30px;
      }
      label {
        color: white;
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
        background-color: #62B0F5;
        width: 100%;
        margin-bottom: 40px;
        border-radius: 30px;
        font-family: 'Oswald', sans-serif;
      }
    </style>
<script>
export default {
// eslint-disable-next-line vue/multi-word-component-names
  name: 'contact_form'
}
</script>