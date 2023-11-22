<template>
  <div id="app">
    <AppHeader />
    <AppMain />
    <AppLyrics />
    <AppMusic />
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";
import "./assets/styles/style.css";
import AppLyrics from "./components/AppLyrics.vue";
import AppMusic from "./components/AppMusic.vue";

export default {
  name: "app",
  components: {
    AppHeader,
    AppMain,
    AppLyrics,
    AppMusic,
  },
};
</script>

<style>
@import "./assets/styles/style.css";
</style>
