<template>
  <p v-if="age > 25">{{ msg }}</p>
  <p v-else>you must be 25years or older to view this message</p>
</template>

<script>
export default {
  name: "Greeting",
  props: ["age"],
  data() {
    return {
      msg: "Good Morning, I wish myself a very best of luck today!",
    };
  },
};
</script>

<style scoped lang="scss">
p:hover {
  color: darken(#cc4444, 15%);
}
</style>
