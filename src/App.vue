<script setup>
import { reactive } from 'vue';

const state = reactive({
  count: 0,})

const increment = () => {
  state.count++;
}
</script>

<template>
  {{ state }} <button @click="increment"> Increment </button>
</template>