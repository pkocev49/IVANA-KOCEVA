<template>
  <section id="whyInvest" style="margin-top: 300px">
    <h1 style="margin-top: 100px; text-align: center">Зошто да почнеш да инвсетираш?</h1>
    <ItemCard :whyInvestItems="whyInvestItems" />
  </section>
</template>
<script>
import whyInvestItems from '../utils/whyInvestItems.js'
import ItemCard from './ItemCard.vue'

export default {
  components: {
    ItemCard
  },
  data() {
    return {
      whyInvestItems: whyInvestItems
    }
  }
}
</script>
<style></style>
