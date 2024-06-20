<template> <div>
  <!-- <TestCicle :addUnit="addUnit"/>
  <Congratulation :addUnit="addUnit"/> -->
  <FlashingMessage message="Hallo Boys" :delay="500"/>
    <!-- <CounterButton @increment="increment" :addUnit="addUnit" />
    <Timer @tick="tellMe" name='timer1':delay="2000"/>
    <Timer @tick="kissMe" name='timer2' :delay="5000"/>
    <PeopleList  /> -->
</div>

</template>

<script>
// import PeopleList from './components/PeopleList.vue'
// import CounterButton from './components/CounterButton.vue';
// import Congratulation from './components/Congratulation';
// import TestCicle from './components/TestCicle';
// import Timer from './components/Timer';
import FlashingMessage from './components/FlashingMessage.vue';
export default {
  name: 'App',
  components: {
  //  PeopleList,
  //  CounterButton,
  //  Congratulation,
  //  TestCicle,
  //  Timer,
   FlashingMessage,

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
        tellMe(name){
        this.name
          console.log(name,'tick');
        },
        kissMe(name){
          
          console.log(name,'kiss');
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
