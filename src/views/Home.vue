<template>
  <div class="home">
    home
    <p>My name is {{ name }} and my age is {{ age }}</p>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'Home',
  setup() {
    console.log('setup');

    let name = 'Kyle';
    let age = 16;

    return {
      name,
      age
    };
  },
};
</script>
