<template>
    <div class="table">
        <div v-for="(player, index) in playerStats" :key="index" class="playerStat">
            <div class="player">
                <p>{{ index+1 }}.</p>
                <p>{{ player[0] }}</p>
            </div>
            <div class="score">
                <p>{{ player[1] }}</p>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        data(){
            return {
                playerStats: [
                    ['Cole Caufield', 150],
                    ['Connor McDavid', 145],
                    ['Sidney Crosby', 130],
                    ['Nick Suzuki', 129],
                    ['Nathan MacKinnon', 124],
                    ['Juraj Slafkovsky', 122],
                    ['David Pastarnak', 117],
                    ['Sebastian Aho', 115],
                    ['Leon Drasaitl', 112],
                    ['Connor Bedard', 109]
                ]
            }
        }
    }
</script>

<style scoped>
    .table {
        width: 30vw;
        height: 60vh;
        background-color: #F99806;
        border-radius: 15px;
    }
    .playerStat {
        display: flex;
        justify-content: space-between;
        align-items: center;
        height: 6vh;
        padding: 0 10px;
        border-bottom: solid;
    }
    .playerStat:last-child{
        border-bottom: none !important;
    }
    .player {
        display: flex;
        margin-left: 10px;
    }
    .score {
        display: flex;
        justify-content: center;
        align-items: center;
        border-left: solid;
        width: 20%;
        height: 100%;
    }
</style>