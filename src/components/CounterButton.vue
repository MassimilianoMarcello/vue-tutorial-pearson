<template>
    <div>
        <h1> This change a {{ number }}</h1>
        <button @click="addUnit">Add a unit</button>
    </div>
   
</template>

<script>
export default {
    name:'CounterButton',

    data(){
        return{
             number: 0,
        }
    },
    methods:{
         addUnit(){
            this.number++
        }
    }
  

    


}

</script>