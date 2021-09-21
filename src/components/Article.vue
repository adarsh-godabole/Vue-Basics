<template>
    <div>
Article Component
<h2 v-bind="$attrs">{{title}}</h2>
<h2>{{likes}}</h2>
<h2>{{isQualified?'Yes':'No'}}</h2>
<h1>My name is {{username}}</h1>

    </div>
</template>

<script>
    export default {
        name:'Article',
        props:{
            title:{
                type:String,
                required:true
            },
            likes:Number,
            isQualified:Boolean
        },
        inheritAttrs:false,
        inject:["username"]
        
    }
</script>

<style scoped>

</style>