<script setup lang="ts">
import ListItem from './components/ListItem.vue'

const randomNumber = Math.floor(Math.random() * 1000 + 100)
</script>

<template>
  <main class="main">
    <ul
      v-for="n in randomNumber"
      :key="n"
      class="hero-list"
    >
      <ListItem />
    </ul>
  </main>
</template>

<style scoped>
.main {
  display: flex;
  flex-direction: column;
}

.hero-list {
  padding: 0;
}
</style>
