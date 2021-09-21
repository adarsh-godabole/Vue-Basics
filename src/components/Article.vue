<template>
    <div>
Article Component
<h2>{{title}}</h2>
<h2>{{likes}}</h2>
<h2>{{isQualified?'Yes':'No'}}</h2>

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
        }
        
    }
</script>

<style scoped>

</style>