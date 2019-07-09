<template>
  <v-app>
    
    <navbar v-if="!isLogged"/>

    <v-content>
      <router-view></router-view>
    </v-content>
  </v-app>
</template>

<script>
import Navbar from './components/Navbar'

export default {
  name: 'App',
  components: {
    Navbar
  },
  
  /**
   * This is temporary, until we implement auth logic.
   */
  computed: {
    isLogged() {
      return this.$router.currentRoute.name == 'login' || this.$router.currentRoute.name == 'register';
    }
  }

}
</script>
