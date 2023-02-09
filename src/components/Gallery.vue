<template>
    <v-card>
      <v-tabs
        color="deep-purple accent-4"
        right
      >
        <v-tab :href="tab-1">Landscape</v-tab>
        <v-tab :href="tab-2">City</v-tab>
      </v-tabs>
          <v-tabs-items v-model="tab">
              <v-tab-item
                  v-for="i in 3"
                  :key="i"
                  :value="'tab-' + i">
                  <img src="../img/1.jpg" alt="">
              </v-tab-item>
          </v-tabs-items>
    </v-card>
  </template>
  <script>
  export default {
    name: 'App',
    components: {
    },
    data: () => ({
        paths: [
            '../img/1.jpg',
            '../img/2.jpg',
            '../img/3.jpg',
            '../img/4.jpg'
        ]
    }),
  };
  </script>
  
  <style>
  body {
    font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
  }
  </style>