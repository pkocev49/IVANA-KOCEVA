<template>
  <section id="card" class="cardContainer">
    <div class="itemDiv" v-for="(item, index) in items" :key="index">
      <img :src="item.icon" alt="icon" class="itemIcon" />
      <span class="itemText">{{ item.title }}</span>
    </div>
  </section>
</template>

<script>
export default {
  props: ['items']
}
</script>

<style scoped>
.itemsList {
  font-size: 15px;
  margin-bottom: 5px;
}
li {
  list-style: none;
}

.itemDiv {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 50px;
  border: 3px solid #3f3f3f;
  border-radius: 15px;
  width: 250px;
  height: 150px;
  margin-bottom: 20px;
  text-align: center;
  font-size: 20px;
}

.cardContainer {
  margin-top: 50px;
  display: flex;
  justify-content: space-evenly;
  flex-wrap: wrap;
  width: 100%;
}

.itemIcon {
  width: 50px; /* Adjust size as needed */
  height: 50px; /* Adjust size as needed */
  margin-bottom: 10px;
}

.itemText {
  font-size: 20px;
  color: #3f3f3f;
}

@media only screen and (min-width: 1080px) {
  .itemsList {
    font-size: 18px;
  }
  .itemDiv {
    width: 300px;
    height: 200px;
  }
}
</style>
