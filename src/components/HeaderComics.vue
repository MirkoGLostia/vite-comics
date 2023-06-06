<script>
export default {
  name: "HeaderComics",
  data() {
    return {
      links: [
        {
          id: 1,
          text: 'CHARACTERS',
          url: '#',
          current: false
        },
        {
          id: 2,
          text: 'COMICS',
          url: '#',
          current: true
        },
        {
          id: 3,
          text: 'MOVIES',
          url: '#',
          current: false
        },
        {
          id: 4,
          text: 'TV',
          url: '#',
          current: false
        },
        {
          id: 5,
          text: 'GAMES',
          url: '#',
          current: false
        },
        {
          id: 6,
          text: 'COLLECTIBLES',
          url: '#',
          current: false
        },
        {
          id: 7,
          text: 'VIDEOS',
          url: '#',
          current: false
        },
        {
          id: 8,
          text: 'FANS',
          url: '#',
          current: false
        },
        {
          id: 9,
          text: 'NEWS',
          url: '#',
          current: false
        },
        {
          id: 10,
          text: 'SHOP',
          url: '#',
          current: false
        }
      ]
    }
  }
}
</script>

<template>
  <header>
    <div class="container">
      <div class="headLogo">
        <img src="./../assets/img/dc-logo.png" alt="logo">
      </div>

      <nav>
        <ul>
          <li v-for="link in links" :key="link.id">
            <a :class="link.current ? 'active' : ''" :href="link.url">{{ link.text }}</a>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<style lang="scss" scoped>
@use './../styles/partials/variables' as v;
@use './../styles/partials/mixins.scss' as *;

header {
  height: 100px;
  border-bottom: 1px solid black;

  .container {
    @include myFlex;
    @include myFlexPosition;

    .headLogo {
      width: 70px;
    }

    ul {
      display: flex;

      li {
        font-size: 16px;

        a {
          color: v.$myBlack;
          padding: 35px 12px;

          &.active,
          &:hover {
            color: v.$myBlue;
          }
        }
      }
    }
  }
}
</style>
