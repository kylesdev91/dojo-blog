<template>
  <div class="home">
    <h1>Home</h1>
    <div v-for="name in names" :key="name">{{ name }}</div>
  </div>
</template>

<script>
import { computed, ref } from '@vue/reactivity';

export default {
  name: 'Home',
  setup() {
    const names = ref(['alex', 'ethan', 'j.j', 'kyle', 'nixon', 'nolan']);
    return { names };
  },
};
</script>
