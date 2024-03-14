<template>
  <div class="todaysGames">
      <p>left arrow</p>
      <GameDate/>
      <GameHeaderElement v-for="n in 5" :key="n"/>
      <p>right arrow</p>
  </div>
</template>

<script lang="js">
    import GameHeaderElement from './GameHeaderElement.vue';
    import GameDate from './GameDate.vue';
    
    export default {
        name: "GameHeader",
        components: {
            GameHeaderElement,
            GameDate
        }
    }
</script>

<style scoped>
  .todaysGames {
    display: flex;
    background-color: #F99806;
    height: 18vh;
    border-radius: 0 0 30px 30px;
  }
</style>
