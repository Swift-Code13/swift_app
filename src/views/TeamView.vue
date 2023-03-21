<template>
    <navbar logo="SwiftAndCodeTeam.png"/>
    <h1>Membres de S&C</h1>
    <team_card></team_card>
</template>

<script>
import navbar from "@/components/navbar.vue";
// @ is an alias to /src
import team_card from '@/components/team-card.vue'
export default {
  name: 'TeamView',
  components: {
    team_card,
    navbar
  }
}
</script>
<style>
  h1{
    text-align: center;
    color: white;
  }
</style>