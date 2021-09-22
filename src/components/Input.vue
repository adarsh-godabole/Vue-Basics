<template>
    <div>
        <input type="text" :value="modelValue" @input="('update:modelValue', $event.target.value)">
    </div>
</template>

<script>
    export default {
        name:'Input',
        props:{
            modelValue: String
        }
    }
</script>

<style scoped>

</style>