<template>
  <div>
    <h1>You clicked {{ addUnit }} times</h1>
    <button @click="$emit('increment')">Add a unit</button>
  </div>
</template>

<script>
export default {
  name: "CounterButton",
  props: ["addUnit"],
};
</script>
