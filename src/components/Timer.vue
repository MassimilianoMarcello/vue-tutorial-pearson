<template>
    <div>
<h1>I am a timer</h1>
    </div>
</template>

<script>

    export default {
        name:'Timer',
        props:['delay','name'],
      created(){
        setInterval(() => {
           this.$emit('tick', this.name) 
        }, this.delay);
      }  
    }
</script>

<style  scoped>

</style>