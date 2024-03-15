<template>
    <h1>Head Stats</h1>
    <div id="stats">
        <div class="statsGroup" id="points">
            <h2>Points</h2>
            <StatsTable/>
        </div>
        <div class="statsGroup" id="buts">
            <h2>Goals</h2>
            <StatsTable/>
        </div>
        <div class="statsGroup" id="passes">
            <h2>Pass</h2>
            <StatsTable/>
        </div>
    </div>
</template>

<script lang="ts">
    import StatsTable from '../HeadStats/StatsTable.vue';
    export default {
        name: 'HeadStats',
        components: {
            StatsTable
        }
    }
</script>

<style scoped>
    h1 {
        margin: 15px 0;
        font-weight: bold;
        text-align: center;
    }
    #stats {
        display: flex;
        justify-content: space-around;
    }
    .statsGroup h2{
        text-align: center;
    }
</style>