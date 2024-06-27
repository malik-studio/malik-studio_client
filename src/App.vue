<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import PrimaryLogo from './components/PrimaryLogo.vue'
</script>

<template>
  <header>
    <div class="header-primary">
      <PrimaryLogo logoContent="Malik Studio" />

      <nav class="header-nav">
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </div>
  </header>

  <RouterView />

  <footer>
    <div class="footer-section-top">
      <nav class="footer-nav">
        <RouterLink class="footer-nav-link" to="/">Home</RouterLink>
        <RouterLink class="footer-nav-link" to="/about">About</RouterLink>
      </nav>
      <img src="./assets/icon/logo_icon_xs_black_svg.svg" alt="malik studio hand logo icon"/>
    </div>

    <div class="footer-section-bottom">
      <p>malik studio</p>
      <p>
        <span>malik studio © 2024</span>
        <span>v13.23.13</span>
      </p>
    </div>
  </footer>
</template>

<style>
.header-primary{
  display: flex;
  flex-flow: row nowrap;
  align-items: center;
  justify-content: space-between;
}

.footer-section-top {
  display: flex;
  flex-flow: row nowrap;
  justify-content: space-between;
}

.footer-nav {
  display: inline-flex;
  flex-flow: column nowrap;
}

.footer-section-bottom {
  display: flex;
  flex-flow: row nowrap;
  justify-content: space-between;
}
</style>
