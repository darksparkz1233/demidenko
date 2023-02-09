<template>
  <v-carousel cycle :show-arrows="false">
    <v-carousel-item
      v-for="(item,i) in items"
      :key="i"
      :src="item.src"
    ></v-carousel-item>
  </v-carousel>
</template>

<script>
  export default {
    data () {
      return {
        items: [
          {
            src: 'http://belgosohota.by/wp-content/uploads/2018/09/15_06_05_05_13_sooruzenia.jpg',
          },
          {
            src: 'https://www.plho.by/images/hunt/01vasilevichi/vasilevishi01.jpg',
          },
          {
            src: 'https://www.plho.by/images/hunt/01vasilevichi/vasilevishi04.jpg',
          },
          {
            src: 'https://www.plho.by/images/hunt/01vasilevichi/vasilevishi02.jpg',
          },
          {
            src: 'http://belgosohota.by/wp-content/uploads/2018/09/18_08_29_03_34_oxdom.jpg'
          }
        ],
      }
    },
  }
</script>
<style >
</style>