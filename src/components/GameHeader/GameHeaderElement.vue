<template>
    <div class="game">
        <div class="status" id="final">
            <p>Final</p>
        </div>
        <div id="teams">
           <div class="team" id="Montreal">
                <img class="teamPic" :src="homePic" alt="home playing team">
                <div class="teamText" id="winning">
                    <p>MTL</p>
                    <p class="score">4</p>  
                </div>
            </div>
            <div class="team" id="Detroit">
                <img class="teamPic" :src="awayPic" alt="away playing team">
                <div  class="teamText">
                    <p>DET</p>
                    <p class="score">2</p>    
                </div>
            </div> 
        </div>
        
    </div>
  </template>
  
  <script lang="ts">
      import montrealLogo from '@/assets/montreal-canadiens-logo.png';
      import detroitLogo from '@/assets/detroit-red-wings-logo.png';
      export default {
          name: "GameHeaderElement",
          data() {
            const teamPictures = {
                    montreal : montrealLogo,
                    detroit :  detroitLogo
            };
            return {
                homePic: teamPictures.montreal,
                awayPic: teamPictures.detroit
            };
          }
      }
  </script>
  
  <style scoped>
    .game {
        border-left: solid;
        border-right: solid;
        padding: 4px 8px;
        width: 20vw;
    }
    .status {
        display: flex;
        align-content: center;
        align-self: center;
        height: 2rem;
        width: 50%;
        padding: 4px 8px;
        border-radius: 10px;
    }
    #final {
        color: black;
        background-color: silver;
    }
    #teams{
        display: flex;
        flex-direction: column;
    }
    .team {
        display: flex;
        justify-content: center;
    }
    #winning p{
        font-weight: bold;

    }
    .teamPic {
        height: 45px;
    }
    .teamText {
        display: flex;
        align-self: center;
    }
    .score {
        margin-left: 10px;
    }
  </style>