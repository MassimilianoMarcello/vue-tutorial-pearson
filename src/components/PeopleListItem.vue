<template>
  <div>
    <h1>{{ person.name }}</h1>
    <p>{{ person.age }}</p>
    <p>{{ person.hairColor }}</p>
  </div>
</template>

<script>
export default {
    name:'PeopleItem',
    props:['person'],
    data(){
    return{
       

    }


    }
}
</script>

<style></style>
