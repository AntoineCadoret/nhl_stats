

<template>
  <header>
    <div class="wrapper">
     <RouterLink to="/"><img alt="NHL logo" class="logo" src="@/assets/nhl-logo.png" width="125" height="125" /></RouterLink>
      <nav>
        <RouterLink to="/schedule">Pool</RouterLink>
        <RouterLink to="/schedule">schedule</RouterLink>
        <RouterLink to="/schedule">Stats</RouterLink>
        <RouterLink to="/schedule">Stanings</RouterLink>
      </nav>
    </div>
    <GameHeader/>
  </header>

  <RouterView />

  <footer>
    <p>@NHLStats</p>
  </footer>
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
    margin-bottom: 10px;
  }
  .wrapper{
    display: flex;
    background-color: rgb(24, 24, 24);
    width: 100vw;
    justify-content: space-between;
    padding: 8px;
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
  img {
    height: 10vh;
    width: 8vw;
  }
  footer {
    background-color : rgb(24, 24, 24);
    color : rgb(194, 192, 192);
    text-align: center;
    padding: 2rem 0;
    margin-top: 2rem;
  }
</style>
