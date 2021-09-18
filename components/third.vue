
<template>
  <div>
    <div class="flex-container">
      <div v-for="card in cards" :key="card.title" :cols="card.flex">
        <div>
          <v-img
            class="img"
            :src="card.src"
            gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
            height="200px"
            width="300px"
          >
            <h5 v-text="card.title"></h5>
          </v-img>
        </div>
      </div>
    </div>
    <div>
      <v-btn rounded class="btn1" color="primary" style=""
        >Create your web page now
      </v-btn>
    </div>
  </div>
</template>

<script>
export default {
  data: () => ({
    cards: [
      {
        title: 'Favorite road trips',
        src: 'https://cdn.vuetifyjs.com/images/cards/road.jpg',
      },
      {
        title: 'Best airlines',
        src: 'https://cdn.vuetifyjs.com/images/cards/plane.jpg',
      },
    ],
  }),
}
</script>

<style scoped>
.flex-container {
  display: flex;

  justify-content: center;
  width: 1000px;
  margin-top: 08%;
}
.flex-container > div {
  margin-left: 50px;
}
.img {
  border-radius: 10px;
}
h5 {
  text-align: center;
  margin-top: 30%;
  color: white;
}
.btn1 {
  margin-top: 50px;
  margin-left: 40%;
  text-transform: none;
}
</style>