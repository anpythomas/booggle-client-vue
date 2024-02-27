<script setup>
import { ref } from 'vue'

defineProps({
  msg: String,
})

const count = ref(0)
</script>

<template>
  <h1>{{ msg }}</h1>

  <div class="card">
    <input class="searchBox" type="text">
    <button type="button" @click="count++">search</button>
  </div>

  <p class="read-the-docs">Search a bottle by distillery, release, and/or vintage</p>
</template>

<style scoped>
.read-the-docs {
  color: #888;
}
</style>
