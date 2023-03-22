<template>
    <div class="container">
      <div class="header">
        <h1>Swift & Code</h1>
        <p>Notre mission est de créer des sites web innovants et modernes</p>
      </div>
      <div class="content">
        <div class="block block-1">
          <h2>À propos de nous</h2>
          <p>Nous sommes une startup spécialisée dans la création de sites web modernes et innovants. Nous travaillons avec les dernières technologies pour offrir des sites web rapides, performants et esthétiques.</p>
        </div>
        <div class="block block-2">
          <h2>Nos services</h2>
          <ul>
            <li>Conception et développement de sites web</li>
            <li>Référencement naturel</li>
            <li>Hébergement et maintenance</li>
            <li>Optimisation des performances</li>
          </ul>
        </div>
        <div class="block block-3">
          <h2>À propos de nous</h2>
          <p>Nous sommes une startup spécialisée dans la création de sites web modernes et innovants. Nous travaillons avec les dernières technologies pour offrir des sites web rapides, performants et esthétiques.</p>
        </div>
        <div class="block block-4">
          <h2>À propos de nous</h2>
          <p>Nous sommes une startup spécialisée dans la création de sites web modernes et innovants. Nous travaillons avec les dernières technologies pour offrir des sites web rapides, performants et esthétiques.</p>
        </div>
      </div>
    </div>
  </template>
  
  <style scoped>

    .container {
      max-width: 800px;
      margin: auto;
      font-family: Arial, sans-serif;
      color: #333;
    }
  
    h1 {
      color: white;
      font-size: 48px;
      text-align: center;
      text-shadow: 0 0 0 #ff9100;
      animation: text-shadow-glow 2s ease-in-out infinite;
      transition: all 0.3s ease-in-out;
    }
  
    h1:hover {
      transform: scale(1.1);
      text-shadow: 0 0 20px #ff9100;
    }
  
    .header p {
      font-size: 24px;
      margin-bottom: 0;
    }
  
    .content {
      padding: 20px;
      margin-top: 20px;
    }
  
    .content h2 {
      font-size: 28px;
      margin-top: 0;
    }
  
    .content ul {
      margin: 0;
      padding: 0;
      list-style: none;
    }
  
    .content li {
      margin-bottom: 10px;
    }
  
    .content a {
      color: #ff9100;
    }
  
    .block {
      width: 50%;
      height: 200px;
      display: flex;
      justify-content: center;
      align-items: center;
      float: left;
      margin-right: 4%;
      box-sizing: border-box;
      padding: 20px;
    }
  
    .block-1 {
      background-color: #ff9100;
      animation: move-up-down 2s ease-in-out infinite alternate;
    }
  
    .block-2 {
      color: #ccc;
      background-color: #333;
      animation: move-up-down 2s ease-in-out infinite alternate-reverse;
      float: right;
      margin-right: 0;
      margin-left: 8%;
    }
    .block-3 {
      background-color: #ff9100;
      animation: move-up-down 2s ease-in-out infinite alternate;
    }
    .block-4 {
      color: #ccc;
      background-color: #333;
      animation: move-up-down 2s ease-in-out infinite alternate-reverse;
      float: right;
      margin-right: 0;
      margin-left: 8%;
    }
  
    @keyframes move-up-down {
      0% {
        transform: translateY(0);
      }
      100% {
        transform: translateY(10px);
      }
    }
  </style>
  
  <script>
  export default {
    name: 'presCard'
  }
  </script>