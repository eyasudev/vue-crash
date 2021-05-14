<template>
    <button @click="onClick()" :style="{ background: color }" class="btn" >{{text}}</button>    
</template>

<script>
export default {
    name:'Button',
    props:{
        text:{
            type:String,
            default:'Sample Buttn'
        },
        color:{
            type:String,
            default:'Sample Buttn'
        }
    },
    methods: {
        onClick() {
            this.$emit('btn-click');
        }
    }

}
</script>

<style scoped>

</style>