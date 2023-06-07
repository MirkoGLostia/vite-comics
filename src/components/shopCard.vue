<script>
export default {
    name: "shopCard",
    props: {
        details: Object,
    }
}
</script>

<template>
    <section class="cardContainer">
        <img :src="details.thumb">
        <h3>{{ details.series }}</h3>
    </section>
</template>
  
<style lang="scss" scoped>
@use './../styles/partials/variables' as v;
@use './../styles/partials/mixins.scss' as *;

.cardContainer {
    width: calc((100% / 6) - 20px);

    img {
        width: 100%;
        height: 200px;
        object-fit: cover;
        object-position: top;
    }
}
</style>