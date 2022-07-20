<template>
  <div class="home">
    <h1>Home</h1>
    <p>My name is {{ name }} and my age is {{ age }}</p>
    <button @click="handleClick">click me</button>
    <button @click="age++">Add 1 to age</button>
    <input type="text" v-model="name" />
  </div>
</template>

<script>
import { ref } from '@vue/reactivity';

export default {
  name: 'Home',
  setup() {
    // const p = ref('hello');

    const name = ref('Kyle');
    const age = ref(16);

    const handleClick = () => {
      name.value = 'Kate';
      age.value = 13;
    };

    return {
      name,
      age,
      handleClick,
    };
  },
  data() {
    return {
      score: 5,
    };
  },
};
</script>
