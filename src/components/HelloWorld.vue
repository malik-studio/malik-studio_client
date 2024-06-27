<script setup lang="ts">

defineProps<{
  logoContent: string
}>()
</script>

<template>
  <div class="greetings">
    <img src="../assets/icon/logo_icon_xs_black_svg.svg" alt="malik studio hand logo icon"/>
    <p>{{ logoContent }}</p>
  </div>
</template>
