<template>
    <div>
<h1>I am a timer</h1>
    </div>
</template>

<script>

    export default {
        name:'Timer',
        props:['delay'],
      created(){
        setInterval(() => {
           this.$emit('tick') 
        }, delay);
      }  
    }
</script>

<style  scoped>

</style>