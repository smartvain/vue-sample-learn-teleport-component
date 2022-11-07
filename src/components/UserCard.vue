<template>
  <div class="user-card">
    <p>John Komarnicki</p>
    <span>Front-End Developer</span>
    <BaseModal />
  </div>
</template>

<script setup lang="ts">
import BaseModal from './BaseModal.vue'
</script>

<style scoped lang="scss">
.user-card {
  padding: 20px;
  background-color: rgb(0, 55, 65);
  border-radius: 4px;

  p {
    font-size: 24px;
    margin-bottom: 8px;
  }
}
</style>