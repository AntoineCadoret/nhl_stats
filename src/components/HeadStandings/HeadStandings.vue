<template class="headStanding">
    <h1>Head Standings</h1>
    <div class="standings">
       <div class="conference">
            <div class="division">
                <h2>Atlantic</h2>
                <div class="standing">
                    <div class="standingElement first">
                        <div class="team">
                            <p>1.</p>
                            <img :src="montrealLogo" alt="canadiens">
                            <p class="teamName">Montreal</p>
                        </div>
                        <div class="score">130</div>
                    </div>
                    <div class="standingElement">
                        <div class="team">
                            <p>2.</p>
                            <img :src="detroitLogo" alt="detroit">
                            <p class="teamName">Detroit</p>
                        </div>
                        <div class="score">115</div>
                    </div>
                    <div class="standingElement last">
                        <div class="team">
                            <p>3.</p>
                            <img :src="bostonLogo" alt="boston">
                            <p class="teamName">Boston</p>
                        </div>
                        <div class="score">100</div>
                    </div>
                </div>
            </div>
            <div class="division">
                <h2>Metropolitan</h2>
                <div class="standing">
                    <div class="standingElement first">
                        <div class="team">
                            <p>1.</p>
                            <img :src="montrealLogo" alt="canadiens">
                            <p class="teamName">Montreal</p>
                        </div>
                        <div class="score">130</div>
                    </div>
                    <div class="standingElement">
                        <div class="team">
                            <p>2.</p>
                            <img :src="detroitLogo" alt="detroit">
                            <p class="teamName">Detroit</p>
                        </div>
                        <div class="score">115</div>
                    </div>
                    <div class="standingElement last">
                        <div class="team">
                            <p>3.</p>
                            <img :src="bostonLogo" alt="boston">
                            <p class="teamName">Boston</p>
                        </div>
                        <div class="score">100</div>
                    </div>
                </div>
            </div>
        </div>
        <div class="conference">
            <div class="division">
                <h2>Central</h2>
                <div class="standing">
                    <div class="standingElement first">
                        <div class="team">
                            <p>1.</p>
                            <img :src="montrealLogo" alt="canadiens">
                            <p class="teamName">Montreal</p>
                        </div>
                        <div class="score">130</div>
                    </div>
                    <div class="standingElement">
                        <div class="team">
                            <p>2.</p>
                            <img :src="detroitLogo" alt="detroit">
                            <p class="teamName">Detroit</p>
                        </div>
                        <div class="score">115</div>
                    </div>
                    <div class="standingElement last">
                        <div class="team">
                            <p>3.</p>
                            <img :src="bostonLogo" alt="boston">
                            <p class="teamName">Boston</p>
                        </div>
                        <div class="score">100</div>
                    </div>
                </div>
            </div>
            <div class="division">
                <h2>Pacific</h2>
                <div class="standing">
                    <div class="standingElement first">
                        <div class="team">
                            <p>1.</p>
                            <img :src="montrealLogo" alt="canadiens">
                            <p class="teamName">Montreal</p>
                        </div>
                        <div class="score">130</div>
                    </div>
                    <div class="standingElement">
                        <div class="team">
                            <p>2.</p>
                            <img :src="detroitLogo" alt="detroit">
                            <p class="teamName">Detroit</p>
                        </div>
                        <div class="score">115</div>
                    </div>
                    <div class="standingElement last">
                        <div class="team">
                            <p>3.</p>
                            <img :src="bostonLogo" alt="boston">
                            <p class="teamName">Boston</p>
                        </div>
                        <div class="score">100</div>
                    </div>
                </div>
            </div>
        </div> 
    </div>
    

</template>

<script lang="ts">
    import montrealLogo from '@/assets/montreal-canadiens-logo.png';
    import detroitLogo from '@/assets/detroit-red-wings-logo.png';
    import bostonLogo from '@/assets/boston-bruins-logo.png';
    export default {
        name: 'HeadStandings',
        data() {
            return {
                montrealLogo,
                detroitLogo,
                bostonLogo
            }
        }
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
        margin-top: 20px;
    }
    .standing {
        background-color: #F99806;
        width: 35vw;
        height: 18vh;
        border-radius: 15px;
    }
    .standingElement {
        display: flex;
        justify-content: space-between;
        height: 6vh;
    }
    .first {
        border-bottom: solid;
    }
    .last {
        border-top: solid;
    } 
    .team {
        display: flex;
        align-items: center;
        justify-content: space-around;
    }
    .team p {
        margin: 20px;
    }
    .team img {
        height: 4vh;
    }
    .score {
        display: flex;
        justify-content: center;
        align-items: center;
        width: 10vw;
        height:100%;
        border-left: solid;
    }
</style>