<script>
export default {
  name: "AppHero",
  data() {
    return {
      image: "one-piece.webp",
    };
  },
  computed: {
    buildImageUrl() {
      return new URL(`../assets/img/${this.image}`, import.meta.url).href;
    },
  },
};
</script>

<template>
  <figure>
    <img :src="buildImageUrl" alt="banner image" />
  </figure>
</template>

<style scoped>
figure {
  text-align: center;
}
img {
  max-width: 100%;
}
</style>
