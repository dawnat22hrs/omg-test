<template>
    <li
        v-for="m in randomNumber"
        :key="m"
        class="item"
    >
            <div class="content">
              {{ Math.floor(Math.random() * 1000) }}
            </div>
          </li>
</template>

<script setup lang="ts">
const randomNumber = Math.floor(Math.random() * 100 + 10)
</script>

<style scoped>
.item {
    list-style-type: none;
    width: 5vw;
    height: 5vw;
    display: flex;
    align-items: center;
    justify-content: center;
}

.content {
    width: 5vw;
    height: 5vw;
    border-radius: 8px;
    background-color: gray;
    display: flex;
    align-items: center;
    justify-content: center;
    border: 1px solid black;
    cursor: default;
    transition: all 0.1s ease-in-out;
    -webkit-transition: all 0.2s ease-in-out;
    font-size: 18px;
}

.content:hover {
    width: calc(5vw * 0.8);
    height: calc(5vw * 0.8);
    font-size: calc(18px * 0.8);
}
</style>