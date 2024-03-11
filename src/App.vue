

<template>
  <header>
    <div class="wrapper">
     <RouterLink to="/"><img alt="NHL logo" class="logo" src="@/assets/nhl-logo.png" width="125" height="125" /></RouterLink>
      <nav>
        <RouterLink to="/about">Pool</RouterLink>
        <RouterLink to="/about">Standings</RouterLink>
        <RouterLink to="/about">Stats</RouterLink>
        <RouterLink to="/about">Schedule</RouterLink>
      </nav>
    </div>
    <GameHeader/>
  </header>

  <RouterView />
</template>

<script lang="ts">
  import { RouterLink, RouterView } from 'vue-router';
  import GameHeader from '@/components/GameHeader/GameHeader.vue';

  export default {
    components: {
      GameHeader
    }
  }
</script>

<style scoped>
  header{
    width: 100vw;
  }
  .wrapper{
    display: flex;
    background-color: rgb(24, 24, 24);
    width: 100vw;
    justify-content: space-between;
  }
  nav {
    padding: 2em;
    display: flex;
    width: 50vw;
    justify-content: space-around;
    align-items: center;
  }
  a {
    color: rgb(194, 192, 192);
    text-decoration: none;
  }
  a:hover {
    text-decoration: underline;
    font-weight: bold;
  }
</style>
