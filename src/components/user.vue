<template>
  <button type="button" @click="onClickAge">increase age</button>
  <p>the user is {{ age }} years old</p>
</template>

<script>
export default {
  name: "user",
  props: ["age"],
  methods: {
    onClickAge() {
      this.$emit("age-change");
    },
  },
};
</script>

<style scoped></style>
