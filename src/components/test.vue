<template>
  <div>
    <!--
        Test 1  / Content 1
        <v-card class="mt-5" tile v-for="(personaje, $index) in personajes" :key="$index">
            <v-img :src="personaje.imagen"></v-img>
            <v-card-title>{{ personaje.nombre }}</v-card-title>
        </v-card>

        Test 2  / Content 2
        <v-container fluid>
            <v-row dense>
                <v-col v-for="personaje in personajes" :key="personaje.nombre" :col="personaje.flex">
                <v-card>
                    <v-img :src="personaje.imagen"> </v-img>
                    <v-card-title v-text="personaje.nombre"></v-card-title>
                </v-card>
                </v-col>
            </v-row>
        </v-container>
    -->
  </div>
</template>

<script>
export default {};
</script>

<style></style>
