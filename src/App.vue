<template>
  <h3>Hey!</h3>
  <Greeting :age="age"></Greeting>
  <user :age="age" @age-change="age++"></user>
</template>

<script>
import Greeting from "@/components/greeting.vue";
import user from "@/components/user.vue";
export default {
  name: "App",
  components: {
    Greeting,
    user,
  },
  data() {
    return {
      age: 20,
    };
  },
};
</script>
