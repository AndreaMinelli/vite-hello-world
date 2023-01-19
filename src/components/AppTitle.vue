<script>
export default {
  name: "AppTitle",
  data() {
    return {
      title: "La mia prima app con Vite!",
    };
  },
};
</script>

<template>
  <header>
    <h1>{{ title }}</h1>
  </header>
</template>

<style scoped>
header {
  text-align: center;
}
h1 {
  color: red;
}
</style>
