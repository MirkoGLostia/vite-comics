<script>
import HeaderMenu from './HeaderMenu.vue';

export default {
  name: "HeaderComics",
  components: {
    HeaderMenu
  }
}
</script>

<template>
  <header class="container flexStyle">
    <div>
      <img src="./../assets/img/dc-logo.png" alt="logo">
    </div>
    <div>
      <HeaderMenu />
    </div>
  </header>
</template>

<style scoped>
.container {
  width: 80%;
  margin: 0 auto;
  padding: 20px;
}

.flexStyle {
  display: flex;
  justify-content: space-between;
}
</style>
