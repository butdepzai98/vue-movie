<template>
  <v-app>
    <!-- NavBar -->
    <NavBar />
    <!-- End NavBar -->
    <v-main>
      <router-view/>
    </v-main>

    <!-- Footer -->
    <Footer />
    <!-- End Footer -->
  </v-app>
</template>

<script>
import NavBar from './components/NavBar.vue';
import Footer from './components/Footer.vue';

export default {
  name: 'App',
  components:{
    NavBar,
    Footer
  },

  data: () => ({
    //
  }),
};
</script>
