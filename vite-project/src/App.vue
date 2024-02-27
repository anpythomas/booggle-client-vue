<script setup>
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <div>
    <a href="https://vuejs.org/" target="_blank">
      <img src="https://web-whisky-live.s3-eu-west-1.amazonaws.com/s3fs-public/styles/uc_product_full/public/8122353-001.JPG?itok=omUtD6Wo" class="logo vue" alt="Vue logo" />
    </a>
  </div>
  <HelloWorld msg="Booggle" />
</template>

<style scoped>
.logo {
  height: 12em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
  border-radius: 120px;
}

.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
  border-radius: 120px;
}
</style>
