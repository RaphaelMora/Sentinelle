<template>
  <header>
    <h1 v-html="headerText"></h1>
  </header>
</template>

<script>
export default {
  name: "AppHeader",
  props: {
    headerText: String,
  },
};
</script>

<style>
@import "../assets/styles/header.css";
</style>
