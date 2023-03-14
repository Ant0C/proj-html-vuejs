<script>
import Hero from './Hero.vue';

export default {
  data() {
    return {
      linksNav: [
        {
          link: 'HOME',
        },
        {
          link: 'SHOP',
        },
        {
          link: 'ABOUT',
        },
        {
          link: 'GALLERY',
        },
        {
          link: 'LOCATIONS',
        },
        {
          link: 'JOURNAL',
        },
        {
          link: 'CONTACT',
        },
      ]
    }
  },
  components: {
    Hero
  }

}
</script>

<template>
  <nav>
    <div class="container">
      <div class="row">
        <div class="col-logo">
          <img src="/img/avada-bakery-logo-retina-200x97.png" alt="logo">
        </div>
        <div class="col-menu">
          <ul>
            <li v-for="el in linksNav">
              <a href="#">{{ el.link }}</a>
            </li>
          </ul>
        </div>
        <div class="col-account">
          ACCOUNT<font-awesome-icon icon="fa-solid fa-cart-shopping" />
        </div>
      </div>
    </div>
  </nav>
  <Hero></hero>
</template>

<style lang="scss" scoped>
@use '../src/style/general.scss' as *;

.row {
  display: flex;
  align-items: center;
  justify-content: space-between;
  font-family: 'Roboto', sans-serif;
  font-weight: 300;

  .col-logo,
  .col-menu,
  .col-account {
    flex-basis: calc(100%/3);
  }

  .col-logo {

    img {
      width: 160px;
      padding: 1.25rem 0rem;
      padding-left: 2.18rem;
    }
  }

  .col-menu {
    ul {
      display: flex;
      gap: 2.37rem;
      color: #5b2ca2;

      li {
        padding: 0.4rem;
        font-size: 0.75rem;
      }
    }
  }

  .col-account {
    padding: 1.25rem 0rem;
    padding-right: 2.18rem;
    text-align: end;
    color: #5b2ca2;
    font-size: 0.75rem;
  }
}
</style>
