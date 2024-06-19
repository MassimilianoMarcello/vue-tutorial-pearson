<template>
  <div>
    <h1 v-if="addUnit==10">Congratulation you clicked 10 times this button!</h1>
  </div>
</template>

<script>
export default {
  name: "Congratulation",
  props: ["addUnit"],
};
</script>

<style scoped></style>
