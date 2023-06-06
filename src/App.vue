<script>
import HeaderComics from './components/HeaderComics.vue'
import MainComics from './components/MainComics.vue';
import FooterComics from './components/FooterComics.vue';

export default {
  components: {
    HeaderComics,
    MainComics,
    FooterComics
  }
}

</script>

<template>
  <header>
    <HeaderComics />
    <MainComics />
    <FooterComics />
  </header>
</template>

<style lang="scss">
@use './styles/partials/variables' as *;
@use './styles/general.scss' as *;
</style>
