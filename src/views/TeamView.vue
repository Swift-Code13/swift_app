<template>
    <h1>Membres de S&C</h1>
    <team_card></team_card>
</template>
<script>
// @ is an alias to /src
import team_card from '@/components/team-card.vue'
export default {
  name: 'TeamView',
  components: {
    team_card
  }
}
</script>
<style>
  h1{
    text-align: center;
    color: white;
  }
</style>