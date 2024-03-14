<template>
    <div>
        <p>{{ week }}</p>
        <p>{{ month }}</p>
        <p>{{ day }}</p>
    </div>
    
</template>
<script>
    export default {
        name: "GameDate",
        data(){
            const date = new Date();
            const weekdays = ["Sun","Mon","Tue","Wed","Thu","Fri","Sat"];
            const months = ["Jan","Feb","Mar","Apr","May","Jun","Jul","Aug","Sep","Oct","Nov","Dec"];
            return {
                week: weekdays[date.getDay()],
                month: months[date.getMonth()],
                day: date.getDate()
            };
        }
    };
</script>

<style scoped>
    div {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        border-left: solid;
        border-right: solid;
        padding: 8px 16px;
    }
    div p {
        font-weight: bold;
        font-size: 1.2em;
    }
</style>