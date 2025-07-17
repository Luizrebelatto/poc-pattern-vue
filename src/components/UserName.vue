<template>
  <div class="user-info">
    <div class="user-name">{{ name }}</div>
    <div class="user-lastname">{{ lastName }}</div>
  </div>
</template>

<script setup>
defineProps({
  name: { type: String, required: true },
  lastName: { type: String, required: true }
})
</script>

<style scoped>
.user-info {
  display: flex;
  flex-direction: column;
}
.user-name,
.user-lastname {
  font-size: 16px;
  font-weight: 500;
}
</style>
