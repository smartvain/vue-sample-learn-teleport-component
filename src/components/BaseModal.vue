<template>
  <button @click="openModal">View User</button>

  <Teleport to="#modal">
    <div class="modal-wrap" v-if="isModalOpen">
      <div class="modal">
        <slot>
          <h1>Vue Teleport</h1>
          <p>This modal is now outside of our vue application!</p>
        </slot>
        <button @click="closeModal">Close</button>
      </div>
    </div>
  </Teleport>
</template>

<script setup lang="ts">
import { ref } from 'vue'

const isModalOpen = ref(false)

const openModal = () => {
  isModalOpen.value = true
}

const closeModal = () => {
  isModalOpen.value = false
}
</script>

<style scoped lang="scss">
</style>