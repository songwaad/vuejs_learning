<script setup>
import { ref } from 'vue';

const currentLink = ref('https://google.com')

const changeLink = () => {
  currentLink.value = 'https://youtube.com'
};
</script>

<template>
  <div>
    <a href="currentLink" target="_blank">Click to go to {{ currentLink }}</a>
    <button @click="changeLink()">Click to change</button>
  </div>
</template>