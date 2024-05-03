<template>
    <li class="item">
        <ul class="list">
          <Item />
        </ul>
      </li>
</template>

<script setup lang="ts">
import Item from './Item.vue'
</script>

<style scoped>
.item {
    list-style-type: none;
}

.list {
    display: flex;
    align-items: center;
    width: 100%;
    padding: 0;
    flex-wrap: wrap;
    gap: 8px;
}
</style>