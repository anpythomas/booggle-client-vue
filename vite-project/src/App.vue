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
  <div id="app">
    <input type="text" v-model="textInput" placeholder="Enter some text...">
    <button @click="sendToAPI">Sent</button>
    <p v-if="apiResponse">{{ apiResponse }}</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      textInput: '', // To hold the text input value
      apiResponse: null, // To store the API response
    };
  },
  methods: {
    async sendToAPI() {
      const url = 'http://booggleapi6-dev.us-west-2.elasticbeanstalk.com/bottles'; // Replace with your actual API endpoint
      try {
        const response = await fetch(url, {
          method: 'GET', // or 'GET', depending on your API
          headers: {
            'Content-Type': 'application/json',
          },
        //   body: JSON.stringify({ text: this.textInput }), // Adjust based on your API's expected format
        });
        const data = await response.json(); // Assuming the response is JSON
        console.log(data);
        this.apiResponse = data; // Update apiResponse with the result
      } catch (error) {
        console.error('Error:', error);
        this.apiResponse = 'Failed to fetch data';
      }
    },
  },
}
</script>

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
