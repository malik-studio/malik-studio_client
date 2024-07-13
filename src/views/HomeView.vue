<script setup lang="ts">
import EmailPrimary from '../components/EmailPrimary.vue'
</script>

<template>
  <main class="main-home">
    <h2 class="home-heading-one">
      Digital Provider and Liaison
    </h2>
    <p class="home-heading-one-subtitle">
      <span>
      We design and build solutions for your business
      </span>
      <span>
      and we're damn good
      </span>
    </p>
    <EmailPrimary />
  </main>
</template>

<style scoped>
.main-home {
  display: flex;
  flex-flow: column nowrap;
  align-items: center;
  justify-content: center;
}

.home-heading-one-subtitle {
  display: flex;
  flex-flow: column nowrap;
  align-items: center;
  justify-content: center;
}
</style>
