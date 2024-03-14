<template>
  <div class="todaysGames">
      <p>left arrow</p>
      <p>date</p>
      <GameHeaderElement v-for="n in 4" :key="n"/>
      <p>right arrow</p>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import GameHeaderElement from './GameHeaderElement.vue';
    
    export default defineComponent ({
        name: "GameHeader",
        components: {
            GameHeaderElement
        }
    })
</script>

<style scoped>
  .todaysGames {
    display: flex;
    background-color: #F99806;
    height: 15vh;
    border-radius: 0 0 30px 30px;
  }
</style>
