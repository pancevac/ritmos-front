<template>
  <div class="team">

    <v-container fluid grid-list-lg>

      <h1 style="margin: 20px">Latest albums</h1>

      <v-layout row wrap>
        <v-flex xs12 sm6 md4 lg3 v-for="person in team" :key="person.name">
          <card/>
        </v-flex>
      </v-layout>

      <h1 style="margin: 20px">Latest songs</h1>

      <v-layout row wrap>
        <v-flex xs12 sm6 md4 lg3 v-for="person in team" :key="person.name">
          <card/>
        </v-flex>
      </v-layout>

    </v-container>
    
  </div>
</template>

<script>
import Card from '../components/Card'

export default {

  components: {
    Card
  },

  data() {
    return {
      team: [
        { name: 'The Net Ninja', role: 'Web developer', avatar: '/avatar-1.png' },
        { name: 'Ryu', role: 'Graphic designer', avatar: '/avatar-2.png' },
        { name: 'Chun Li', role: 'Web developer', avatar: '/avatar-3.png' },

      ]
    }
  }
}
</script>