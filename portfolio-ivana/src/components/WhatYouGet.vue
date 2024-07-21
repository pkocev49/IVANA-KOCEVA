<template>
  <section>
    <h1 class="title">{{ title }}</h1>
    <Card :items="items" />
  </section>
</template>

<script>
import Card from './Card.vue'
import items from '../utils/items.js'

export default {
  components: {
    Card
  },
  data() {
    return {
      title: 'Што добивате вие?',
      items: items
    }
  }
}
</script>

<style scoped>
.title {
  text-align: center;
  margin-top: 100px;
}
</style>
