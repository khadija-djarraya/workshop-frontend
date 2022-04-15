<template>
  <v-app>
    hello world
  <v-card
    max-width="450"
    class="mx-auto"
  >
    <v-list three-line>

        <v-list-item v-for="movie in movies" :key ="movie">
          <v-list-item-content>
            <v-list-item-title>{{movie.Title}}</v-list-item-title> <!-- this is the title of the card -->
            <v-list-item-subtitle>{{movie.Subtitle}} </v-list-item-subtitle> <!-- this is the subtitle of the card -->
          </v-list-item-content>
        </v-list-item>

    </v-list>
  </v-card>
  </v-app>
</template>

<script>

export default {
  name: 'App',

  components: {
  },

  data: () => ({
    movies:[]
  }),
  mounted(){

  }
};
</script>
