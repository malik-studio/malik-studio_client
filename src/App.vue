<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import HeaderLogo from './components/HeaderLogo.vue'
</script>

<template>
  <header>
    <div class="header-wrapper">
      <HeaderLogo logoContent="Malik Studio" />

      <nav class="header-nav">
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </div>
  </header>

  <RouterView />

  <footer>
    <div>
      <div class="footer-section-top">
        <nav class="footer-nav">
          <RouterLink class="footer-nav-link" to="/">Home</RouterLink>
          <RouterLink class="footer-nav-link" to="/about">About</RouterLink>
        </nav>
        <img class="footer-logo-image" src="./assets/icon/logo_icon_xs_white_svg.svg" alt="malik studio hand logo icon" />
      </div>
      <div class="footer-section-bottom">
        <p>malik studio</p>
        <p>
          <span>malik studio © 2024</span>
          <span>v13.23.13</span>
        </p>
      </div>
    </div>
  </footer>
</template>

<style scoped>
header {
  position: sticky;
  top: 0;

  padding: 1rem 2rem 0;
}

.header-wrapper {
  display: flex;
  flex-flow: row nowrap;
  align-items: center;
  justify-content: space-between;
}

footer {
  padding: 0 2rem 1rem;

  background-color: #2A2A2A;
}

.footer-section-top {
  position: relative;
  display: flex;
  flex-flow: row nowrap;
  justify-content: space-between;

  padding: 1rem 0 0;
}

.footer-nav {
  display: inline-flex;
  flex-flow: column nowrap;
}

.footer-section-bottom {
  display: flex;
  flex-flow: row nowrap;
  justify-content: space-between;

  color: white;
}
</style>
