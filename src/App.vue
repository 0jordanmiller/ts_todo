<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <p>testing</p>
  </div>
</template>

<script lang="ts">
import Vue from "vue";
import { User } from "../types";

export default Vue.extend({
  name: "App",
  data() {
    return {
      int: 1 as number,
      user: {
        firstName: "Pat",
        lastName: "Miller",
        location: {
          city: "Minneapolis",
          state: "Minnesota",
        },
      } as User,
    };
  },
});
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
