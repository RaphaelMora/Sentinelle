<template>
  <div>
    <button class="boutonLyrics" @click="toggleLyrics">Lyrics</button>
    <textarea
      v-if="showLyrics"
      id="story"
      name="story"
      rows="5"
      cols="33"
      v-model="text"
      readonly
    ></textarea>
  </div>
</template>

<script>
export default {
  data() {
    return {
      text: `Si c'était à refaire,
je referais tout
J'effacerais ces larmes sur tes joues
Je te dirais reviens
Cette fois, je ferai les choses bien
Cette fois, je serai heureux
Dans le ciel de tes yeux bleus
Dans le creux de tes deux mains
On se voit toujours demain
Dans le ciel de tes yeux bleus
Dans le creux de tes deux mains
Confirme-moi pour demain

Est-ce que tu regrettes?
Moi pas
Même, pas du tout
Est-ce que tu regrettes?
Moi, absolument pas
Pas du tout

Si c'était à refaire,
je referais tout
Mais tout ce que j'ai fait,
je le changerais
sans rien changer à ma vie
Je resterais qui je suis
Tout en étant différent,
sans rien changer pour autant
Mais en changeant totalement,
sans bouleverser mes acquis
Tout en étant différent,
mais en changeant totalement
Sans bouleverse mes acquis,
si tu peux pas demain j'peux jeudi

Est-ce que tu regrettes?
Tu t'es moquée de moi et de ma confiance
ça m'apprendra à faire un peu trop confiance
Je suis trop honnête
Alors que toi,
non
Pas du tout

Alors, est-ce que tu regrettes?
Eh bien moi pas du tout
Mais retourne-toi,
cesse donc ta mascarade
Et sèche donc ton mascara
Et arrête donc avec toutes ces escalades 
pendant que moi, je fais des-des,
arrête
D'ailleurs tu peux jeudi?
Parce que moi je peux

Pas du tout
Du tout`,
      showLyrics: false,
    };
  },
  methods: {
    toggleLyrics() {
      this.showLyrics = !this.showLyrics;
    },
  },
};
</script>

<style>
@import "../assets/styles/lyrics.css";
</style>
