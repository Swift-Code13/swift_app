<template>
<div class="navbarsetc">
    <nav class="navbar navbar-expand-lg navbar-dark bg-black">
      <router-link to="/"><img :src="require(`@/assets/${logo}`)"></router-link>
  <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
    <span class="navbar-toggler-icon"></span>
  </button>
  <div class="collapse navbar-collapse" id="navbarNav">
    <ul class="navbar-nav">
      <li class="nav-item" :class="{ active: isActive('/presentation') }">
        <router-link to="presentation" class="nav-link">Présentation</router-link>
      </li>
      <li class="nav-item" :class="{ active: isActive('/projects') }">
        <router-link to="projects" class="nav-link">Projets</router-link>
      </li>
      <li class="nav-item" :class="{ active: isActive('/team') }">
        <router-link to="team" class="nav-link">L'équipe</router-link>
      </li>
      <li class="nav-item" :class="{ active: isActive('/contact') }">
        <router-link to="contact" class="nav-link">Contact</router-link>
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
  },
  props: {
    logo: String
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