<template>
    <HeadStandings/>
    <HeadStats/>
</template>

<script lang="ts">
    import HeadStandings from '../HeadStandings/HeadStandings.vue';
    import HeadStats from '../HeadStats/HeadStats.vue';

    export default { 
        name: 'HeadPage',
        components: {
            HeadStandings,
            HeadStats
        }
    }
</script>
