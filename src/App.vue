<template>
  <v-app>
    <!-- nav -->
    <v-app-bar dense class="red lighten-1">
      <v-toolbar-title class="white--text"
        >Rick & Morty Personajes</v-toolbar-title
      >
      <v-spacer></v-spacer>
    </v-app-bar>

    <!-- content 3 -->
    <v-container>
      <v-row no-gutters>
        <v-col
          v-for="(personaje, $index) in personajes"
          :key="$index"
          cols="12"
          sm="4"
        >
          <v-card class="pa-2" outlined tile>
            <v-img :src="personaje.imagen"></v-img>
            <v-card-title>{{ personaje.nombre }}</v-card-title>
          </v-card>
        </v-col>
      </v-row>
    </v-container>

    <!-- content 1 -->
    <!-- content 2 -->

    <!-- footer -->
    <v-footer padless>
      <v-card flat tile width="100%" class="red lighten-1 text-center">
        <v-divider></v-divider>
        <v-card-text class="white--text">
          {{ new Date().getFullYear() }} — <strong>Rick & Morty</strong>
        </v-card-text>
      </v-card>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  name: "App",
  data: () => ({
    personajes: [
      {
        id: 1,
        nombre: "Morty",
        imagen: "https://rickandmortyapi.com/api/character/avatar/2.jpeg",
        flex: 6,
      },
      {
        id: 2,
        nombre: "Rick",
        imagen: "https://rickandmortyapi.com/api/character/avatar/1.jpeg",
        flex: 6,
      },
      {
        id: 3,
        nombre: "Summer",
        imagen: "https://rickandmortyapi.com/api/character/avatar/3.jpeg",
        flex: 6,
      },
      {
        id: 4,
        nombre: "Beth",
        imagen: "https://rickandmortyapi.com/api/character/avatar/4.jpeg",
        flex: 6,
      },
      {
        id: 5,
        nombre: "Jerry",
        imagen: "https://rickandmortyapi.com/api/character/avatar/5.jpeg",
        flex: 6,
      },
    ],
  }),
};
</script>

<style></style>
