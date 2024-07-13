<script setup lang="ts">

defineProps<{
  logoContent: string
}>()
</script>

<template>
  <div class="logo_container">
    <img class="header-logo-image" src="../assets/icon/logo_icon_xs_black_svg.svg" alt="malik studio hand logo icon" />
    <p>{{ logoContent }}</p>
  </div>
</template>

<style>

.logo_container {
  display: flex;
  flex-flow: row nowrap;
  align-items: center;
}

.header-logo-image {
  width: 50px;
  height: 50px;
}
</style>
