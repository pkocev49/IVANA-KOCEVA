<template>
  <section id="home" class="top">
    <div class="firstContainer">
      <div>
        <img class="firstImage" src="../../assets/Images/vector.svg" alt="Hero Image" />
      </div>
      <div class="seccondContainer">
        <h2 class="title">{{ title }}</h2>
        <h3 class="subHeading">{{ subHeading }}</h3>
      </div>
    </div>
    <div class="triangle"></div>
  </section>
  <div class="bottom"></div>
  <WhatYouGet />
</template>

<script>
import WhatYouGet from '../WhatYouGet.vue'
export default {
  components: {
    WhatYouGet
  },
  data() {
    return {
      title: 'Придружи се во тимот на успешните',
      subHeading: 'И заработувај многу'
    }
  }
}
</script>

<style scoped>
#home {
  background-color: #3f3f3f !important;
  height: 100vh;
}
h2 {
  color: white;
}
h3 {
  color: white;
}

li {
  list-style: none;
  color: white;
}

.seccondContainer {
  padding: 20px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
.title {
  margin-top: 40%;
  margin-bottom: 20px;
  font-weight: bold;
  font-size: 30px;
  text-align: center;
}
.subHeading {
  text-decoration: underline;
}
.itemsList {
  font-size: 15px;
  margin-bottom: 5px;
}

.firstImage {
  width: 300px;
  border-radius: 30px;
  display: none;
  margin-top: 40%;
}
@media only screen and (min-width: 768px) {
  .firstImage {
    display: block;
  }
  .firstContainer {
    display: flex;
    flex-direction: row-reverse;
    justify-content: space-evenly;
    align-items: center;
  }
}
@media only screen and (min-width: 1080px) {
  .firstImage {
    width: 500px;
  }
  .title {
    font-size: 40px;
  }
}

/* .top {
  height: 100px;
  width: 100%;
} */
/* .bottom {
  height: 200px;
  width: 100%;
}
.triangle {
  border-top: 250px solid #3f3f3f;
  border-left: 3400px solid transparent;
  border-right: 0px solid transparent;
  bottom: -600px;

  width: 0;
  height: 0;
  top: 107px;
  content: '';
  display: block;
  position: absolute;
  overflow: hidden;
  left: 20;
  right: 0;
  margin: auto;
} */
</style>
