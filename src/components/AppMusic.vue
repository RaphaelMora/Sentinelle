<template>
  <div>
    <button class="boutonMusic" @click="toggleSound">
      {{ isPlaying ? "Pause" : "Balance le son" }}
    </button>
    <audio ref="player" src="../../public/son.mp3"></audio>
  </div>
</template>

<script>
export default {
  data() {
    return {
      isPlaying: false,
    };
  },
  methods: {
    toggleSound() {
      if (this.isPlaying) {
        this.$refs.player.pause();
      } else {
        this.$refs.player.play();
      }
      this.isPlaying = !this.isPlaying;
    },
  },
};
</script>

<style>
@import "../assets/styles/music.css";
</style>
