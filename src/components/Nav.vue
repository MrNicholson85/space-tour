<template>
  <div class="header">
    <div class="logo">
      <img :src="logoImage"/>
    </div>
    <nav>
      <ul id="primary-navigation" class="primary-navigation">
        <li>
          <router-link to="/">
            <span aria-hidden="true">00 </span>Home
          </router-link>
        </li>
        <li>
          <router-link to="/destionation">
            <span aria-hidden="true">01 </span>Destination
          </router-link>
        </li>
        <li>
          <router-link to="/crew">
            <span aria-hidden="ture">02 </span>Crew
          </router-link>
        </li>
        <li>
          <router-link to="/technology">
            <span aria-hidden="true">03 </span>Technology
          </router-link>
        </li>
      </ul>
    </nav>
  </div>
</template>
<script>
import logoImage from '@/assets/images/space_tour_logo.svg'

export default {
  name: 'App',
  data () {
    return {
      logoImage
    }
  }
}
</script>
<style lang="scss">
  @import '@/assets/scss/typography.scss';

  .header {
    display: flex;
    align-items: center;

    .logo {
       margin: 1rem;
    }

    nav {
      ul {
        display: flex;
        list-style: none;
        column-gap: 48px;
        width: 818px;
        background: rgba($white, .4);
        backdrop-filter: blur(10px);
        justify-content: center;

        li {
          height: 96px;
          display: flex;
          align-items: center;
        }

        a {
          color: $white;
          text-decoration: none;
          span {
            font-weight: bold;
          }
        }
      }
    }
  }
</style>
