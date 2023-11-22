<template>
  <article>
    <AppHeader class="h1" :headerText="headerText"></AppHeader>
    <button class="boutonArticle" @click="changeHeaderText">
      Alors que moi
    </button>
    <p class="p1" v-if="showParagraph">PAS DU TOUT !</p>
    <img
      class="image2"
      v-if="showImage"
      src="../../public/images2.jpg"
      alt=""
    />
  </article>
</template>

<script>
import AppHeader from "./AppHeader.vue";

export default {
  data() {
    return {
      headerText: "Est-ce que tu regrette ?",
      showParagraph: false,
      showImage: false,
    };
  },
  components: {
    AppHeader,
  },
  methods: {
    changeHeaderText() {
      this.headerText =
        "🎵<span class='h1text'>Tu t'es moqué de moi et de ma confiance</span> <br> <span class='h1dubas'>ça m'apprendra à faire un peu trop confiance</span>🎵";

      this.showParagraph = true;
      this.showImage = true;
    },
  },
};
</script>

<style>
@import "../assets/styles/article.css";
</style>
