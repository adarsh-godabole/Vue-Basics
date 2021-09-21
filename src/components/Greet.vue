<template>
    <div>
Hello {{Uname}} your color is {{color}}
    </div>
</template>

<script>
    export default {
        name:"Greet",
        props:['Uname','color']
    }
</script>

<style scoped>

</style>