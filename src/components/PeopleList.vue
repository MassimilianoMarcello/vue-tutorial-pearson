<template>
  <div>
    <PeopleListItem :person="person1" />
    <PeopleListItem :person="person2" />
    <PeopleListItem :person="person3" />
  </div>
</template>

<script>
import PeopleListItem from "./PeopleListItem.vue";

export default {
  name: "PeopleList",
  components: {
    PeopleListItem,
  },
  data(){
return{
    person1:{name:'Aldous', age:33, hairColor:'brown'},
 person2:{name:'Rino', age:63, hairColor:'red'},
 person3:{name:'Lazarus', age:39, hairColor:'green'},
}

}
  }

</script>

<style></style>
