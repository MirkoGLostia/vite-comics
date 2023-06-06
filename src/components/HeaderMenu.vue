<script>
export default {
  name: "HeaderMenu"
}
</script>

<template>
  <section class="flexStyle menuContainer">
    <div>
      <span>
        characters
      </span>
    </div>

    <div>
      <span>
        comics
      </span>
    </div>

    <div>
      <span>
        movies
      </span>
    </div>

    <div>
      <span>
        tv
      </span>
    </div>

    <div>
      <span>
        games
      </span>
    </div>

    <div>
      <span>
        collectibles
      </span>
    </div>

    <div>
      <span>
        videos
      </span>
    </div>

    <div>
      <span>
        fans
      </span>
    </div>

    <div>
      <span>
        news
      </span>
    </div>

    <div>
      <span>
        shop
      </span>
    </div>
  </section>
</template>

<style scoped>
.flexStyle {
  height: 100%;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.menuContainer div {
  padding: 20px;
}
</style>