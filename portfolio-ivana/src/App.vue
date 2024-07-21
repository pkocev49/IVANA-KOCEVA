<template>
  <Header />
  <Home />
</template>

<script>
import Header from './components/Layouts/Header.vue'
import Home from './components/pages/Home.vue'
export default {
  components: {
    Header,
    Home
  },
  setup() {}
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,100..900;1,100..900&display=swap');

* {
  font-family: 'Montserrat', sans-serif;
}
</style>
