<template class="headStanding">
    <h1>Head Standings</h1>
    <div class="standings">
       <div class="conference">
            <div class="division">
                <h2>Atlantic</h2>
                <div class="standing">
                    <div class="standingElement first">
                        <div class="team"></div>
                        <div class="score"></div>
                    </div>
                    <div class="standingElement">
                        <div class="team"></div>
                        <div class="score"></div>
                    </div>
                    <div class="standingElement last">
                        <div class="team"></div>
                        <div class="score"></div>
                    </div>
                </div>
            </div>
            <div class="division">
                <h2>Metropolitan</h2>
                <div class="standing">
                    <div class="standingElement first">
                        <div class="team"></div>
                        <div class="score"></div>
                    </div>
                    <div class="standingElement">
                        <div class="team"></div>
                        <div class="score"></div>
                    </div>
                    <div class="standingElement last">
                        <div class="team"></div>
                        <div class="score"></div>
                    </div>
                </div>
            </div>
        </div>
        <div class="conference">
            <div class="division">
                <h2>Central</h2>
                <div class="standing">
                    <div class="standingElement first">
                        <div class="team"></div>
                        <div class="score"></div>
                    </div>
                    <div class="standingElement">
                        <div class="team"></div>
                        <div class="score"></div>
                    </div>
                    <div class="standingElement last">
                        <div class="team"></div>
                        <div class="score"></div>
                    </div>
                </div>
            </div>
            <div class="division">
                <h2>Pacific</h2>
                <div class="standing">
                    <div class="standingElement first">
                        <div class="team"></div>
                        <div class="score">100</div>
                    </div>
                    <div class="standingElement">
                        <div class="team"></div>
                        <div class="score">100</div>
                    </div>
                    <div class="standingElement last">
                        <div class="team"></div>
                        <div class="score">100</div>
                    </div>
                </div>
            </div>
        </div> 
    </div>
    

</template>

<script lang="ts">
    export default {
        name: 'HeadStandings'
    }
</script>

<style scoped>
    h1{
       text-align: center;
       font-weight: bold;
    }
    .standings {
        display: flex;
        justify-content: space-around;
    }
    .division {
        text-align: center;
    }
    .standing {
        background-color: #F99806;
        width: 35vw;
        height: 18vh;
        border-radius: 15px;
    }
    .standingElement {
        height: 6vh;
    }
    .first {
        border-bottom: solid;
    }
    .last {
        border-top: solid;
    } 
    .score {
        float: right;
        width: 10vw;
        height:100%;
        border-left: solid;
    }
</style>