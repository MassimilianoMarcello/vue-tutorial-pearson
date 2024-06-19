<template>
  <div>
    <h1 v-if="addUnit==15">This is a life cicle test</h1>
  </div>
</template>

<script>
export default {
    name:'TestCycle',
    props:['addUnit'],

    beforeCreate(){
        console.log('before create');
    },
created(){
        console.log('created');
    },

beforeMount(){
        console.log('before mounted');
    },
mounted(){
        console.log('created');
    },
    beforeUpdate(){
        console.log('before update');
    },
updated(){
        console.log('updated');
    },
    unmounted(){
        console.log('unmounted');
    }
}
</script>

<style scoped>

</style>
