<template>
    <br><center><h1>Formulaire de contact</h1></center><br>
    <form method="post" action="process.php">
      <input type="text" id="name" name="name" placeholder="Nom" required>

      <input type="email" id="email" name="email" placeholder="Email" required>

      <input type="text" id="subject" name="subject" placeholder="Sujet" required>

      <textarea id="message" name="message" rows="5" placeholder="Message" required></textarea>

      <center><input type="submit" value="Envoyer"></center>
    </form>
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
        border: 1px solid #ccc;
        box-sizing: border-box;
        margin-bottom: 10px;
        resize: vertical;
        border-radius: 20px;
        color: white;
      }
      input[type="text"], input[type="email"], textarea{
        background-color: black;
      }

      input::placeholder, textarea::placeholder {
        color: #989797;
      }
      input[type="submit"] {
        background-color: #ff9100;
        color: white;
        padding: 10px 20px;
        border: none;
        border-radius: 4px;
        cursor: pointer;
        border-radius: 20px;
      }
      input[type="submit"]:hover {
        background-color: #ff7b66;
        transition: 0.7s;
      }
    </style>
<script>
export default {
// eslint-disable-next-line vue/multi-word-component-names
  name: 'contact_form'
}
</script>