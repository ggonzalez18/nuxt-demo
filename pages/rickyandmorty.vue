<template>
  <v-row>
    <v-col cols="12" sm="8" offset-sm="2">
      <v-card>
        <v-container fluid>
          <v-row>
            <v-col
              v-for="personaje in personajes"
              :key="personaje.id"
              class="d-flex child-flex"
              cols="4"
            >
              <v-card tile class="d-flex flex-column">
                <v-img :src="personaje.image" aspect-ratio="1" class="grey lighten-2" />
                <v-card-title>{{ personaje.name }}</v-card-title>
              </v-card>
            </v-col>
          </v-row>
        </v-container>
      </v-card>
    </v-col>
  </v-row>
</template>

<script>
export default {
  name: 'Rickyandmorty',
  data () {
    return {
      personajes: [
        {
          id: 1,
          name: 'Morty',
          image: 'https://rickandmortyapi.com/api/character/avatar/2.jpeg'
        },
        {
          id: 2,
          name: 'Rick',
          image: 'https://rickandmortyapi.com/api/character/avatar/1.jpeg'
        },
        {
          id: 3,
          name: 'Summer',
          image: 'https://rickandmortyapi.com/api/character/avatar/3.jpeg'
        },
        {
          id: 4,
          name: 'Beth',
          image: 'https://rickandmortyapi.com/api/character/avatar/4.jpeg'
        },
        {
          id: 5,
          name: 'Jerry',
          image: 'https://rickandmortyapi.com/api/character/avatar/5.jpeg'
        }
      ]
    }
  }
}
</script>

<style>

</style>
