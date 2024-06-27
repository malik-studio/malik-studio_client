<script setup lang="ts">

defineProps<{
  logoContent: string
}>()
</script>

<template>
  <div class="logo_container">
    <img src="../assets/icon/logo_icon_xs_black_svg.svg" alt="malik studio hand logo icon" class="logo_image"/>
    <p>{{ logoContent }}</p>
  </div>
</template>

<style>

.logo_container {
  display: flex;
  flex-flow: row nowrap;
  align-items: center;
}

.logo_image {
  width: 50px;
  height: 50px;
}
</style>
