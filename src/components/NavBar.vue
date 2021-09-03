<template>
  <nav>
      <v-app-bar app color="teal" dark>
        <v-icon class="mr-2">fas fa-video</v-icon>
        <v-toolbar-title>VUE Movies</v-toolbar-title>
        <v-btn text class="ml-2" to="/">Movies</v-btn>
        <v-btn text class="ml-2" to="/actors">Actors</v-btn>
        <v-btn text class="ml-2" to="/profile">Profile</v-btn>
        <v-btn text class="ml-2" to="/contact">Contact</v-btn>

        <v-spacer></v-spacer>
        
        <v-autocomplete
          clearable
          hide-no-data
          hide-selected
          color="white"
          label="search"
          prepend-inner-icon="search"
          flat
        ></v-autocomplete>

        <v-btn icon>
          <v-badge color="green" content="2" overlap>
            <v-icon>far fa-bell</v-icon>
          </v-badge>
        </v-btn>
        <v-avatar size="40">
          <v-img :src="require('../assets/Xavi_Logo.jpeg')"></v-img>
        </v-avatar>
      </v-app-bar>
  </nav>
</template>

<script>
export default {
  data:() => ({
    drawer:null,
    model:'',
  })
}
</script>

<style>

</style>