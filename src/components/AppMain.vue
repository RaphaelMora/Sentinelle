<template>
  <main>
    <section>
      <div class="product-image">
        <img
          class="meme"
          :src="
            image
              ? require('../images/meme.jpg')
              : require('../images/images.jpg')
          "
          alt="les images"
          @mouseover="hoverLink"
          @mouseout="resetImage"
        />
      </div>
      <AppArticle />
    </section>
  </main>
</template>

<script>
import AppArticle from "./AppArticle.vue";

export default {
  components: {
    AppArticle,
  },
  data() {
    return {
      image: false,
    };
  },
  methods: {
    hoverLink() {
      this.image = true;
    },
    resetImage() {
      this.image = false;
    },
  },
};
</script>

<style>
@import "../assets/styles/main.css";
</style>
