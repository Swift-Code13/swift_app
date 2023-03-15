<template>
    <nav class="navbar navbar-expand-lg navbar-light bg-light">
  <a class="navbar-brand" href="/"><img src="../assets/SwiftAndCode.jpeg" alt=""></a>
  <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
    <span class="navbar-toggler-icon"></span>
  </button>
  <div class="collapse navbar-collapse" id="navbarNav">
    <ul class="navbar-nav">
      <li class="nav-item active">
        <a class="nav-link" href="presentation">Présentation<span class="sr-only">(current)</span></a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="projects">Projets Réalisés</a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="team">L'équipe</a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="contact">Contact</a>
      </li>
    </ul>
  </div>
</nav>
</template>
<script>
export default {
// eslint-disable-next-line vue/multi-word-component-names
  name: 'navbar',
}
</script>
<style>
    img{
        height: 50px;
    }
</style>