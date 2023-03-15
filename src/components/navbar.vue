<template>
<div class="navbarsetc">
    <nav class="navbar navbar-expand-lg navbar-dark bg-black">
  <a class="navbar-brand" href="/"><img src="../assets/SwiftAndCode.jpeg" alt=""></a>
  <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
    <span class="navbar-toggler-icon"></span>
  </button>
  <div class="collapse navbar-collapse" id="navbarNav">
    <ul class="navbar-nav">
      <li class="nav-item" :class="{ active: isActive('/presentation') }">
        <a class="nav-link" href="presentation">Présentation</a>
      </li>
      <li class="nav-item" :class="{ active: isActive('/projects') }">
        <a class="nav-link" href="projects">Projets Réalisés</a>
      </li>
      <li class="nav-item" :class="{ active: isActive('/team') }">
        <a class="nav-link" href="team">L'équipe</a>
      </li>
      <li class="nav-item" :class="{ active: isActive('/contact') }">
        <a class="nav-link" href="contact">Contact</a>
      </li>
    </ul>
  </div>
</nav>
</div>
</template>
<script>
export default {
// eslint-disable-next-line vue/multi-word-component-names
  name: 'navbar',
    methods: {
    isActive(route) {
      return this.$route.path === route
    }
  }
}
</script>
<style>
  .nav-item {
    color: #ccc;
  }
  img{
    height: 50px;
  }

  .active {
    font-weight: bold;
  }
</style>