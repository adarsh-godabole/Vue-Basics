<template>
    <div>
        <h2>This is a pop-up</h2>
        <button @click="$emit('close','Adarsh')">Close</button>
    </div>
</template>

<script>
    export default {
        name:'popup',
        emits:['close']
        
    }
</script>

<style scoped>

</style>