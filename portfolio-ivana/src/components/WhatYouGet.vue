<template>
  <section style="margin-top: 300px">
    <h1 class="title">{{ title }}</h1>
    <ItemCard :items="items" />
  </section>
</template>

<script>
import ItemCard from './ItemCard.vue'
import items from '../utils/items.js'
export default {
  components: {
    ItemCard
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
