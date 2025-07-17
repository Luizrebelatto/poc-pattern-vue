<template>
  <div class="user-container">
    <UserAvatarImage :imageUrl="image.imageUrl" />
    <UserName :name="user.name" :lastName="user.lastName" />
  </div>
</template>

<script setup>
import UserAvatarImage from './UserAvatarImage.vue'
import UserName from './UserName.vue'

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
</style>
