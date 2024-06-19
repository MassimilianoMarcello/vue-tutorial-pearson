<template> <div>
  <TestCicle :addUnit="addUnit"/>
  <Congratulation :addUnit="addUnit"/>
    <CounterButton @increment="increment" :addUnit="addUnit" />
    <Timer @tick="tellMe" delay="2000"/>
    <PeopleList  />
</div>

</template>

<script>
import PeopleList from './components/PeopleList.vue'
import CounterButton from './components/CounterButton.vue';
import Congratulation from './components/Congratulation';
import TestCicle from './components/TestCicle';
import Timer from './components/Timer';
export default {
  name: 'App',
  components: {
   PeopleList,
   CounterButton,
   Congratulation,
   TestCicle,
   Timer,

  },
  data(){
        return{
             addUnit: 0,
        }
    },
    methods:{
         increment(){
            this.addUnit++;
        },
        tellMe(){
          console.log('tick');
        }
    }
  
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
