<template>
  <img :src="imageUrl" class="avatar" />
</template>

<script setup>
defineProps({
  imageUrl: { type: String, required: true },
})
</script>

<style scoped>
.avatar {
  width: 64px;
  height: 64px;
  border-radius: 50%;
  object-fit: cover;
}
</style>
