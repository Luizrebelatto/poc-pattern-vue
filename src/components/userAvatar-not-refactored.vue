<template>
  <div class="user-container">
    <img :src="image.imageUrl" :alt="image.description" class="avatar" />
    <div class="user-info">
      <div class="user-name">{{ user.name }}</div>
      <div class="user-lastname">{{ user.lastName }}</div>
    </div>
  </div>
</template>

<script setup>
const user = {
  name: 'Luiz',
  lastName: 'Rebelatto'
}

const image = {
  imageUrl: 'https://i.guim.co.uk/img/media/fe1e34da640c5c56ed16f76ce6f994fa9343d09d/0_174_3408_2046/master/3408.jpg?width=1200&quality=85&auto=format&fit=max&s=1aaf31e276b20b5d12d4bee49c5a99e2',
}
</script>

<style scoped>
.user-container {
  display: flex;
  align-items: center;
  gap: 12px;
}

.avatar {
  width: 64px;
  height: 64px;
  border-radius: 50%;
  object-fit: cover;
}

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
