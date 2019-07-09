<template>
    <v-card color="purple" class="white--text">
              <v-layout row>
                <v-flex xs6>
                  <v-card-title primary-title>
                    <div>
                      <div class="headline">Halycon Days</div>
                      <div>Ellie Goulding</div>
                      <div>(2013)</div>
                    </div>
                  </v-card-title>
                </v-flex>
                <v-flex xs6>
                  <v-img
                    src="https://cdn.vuetifyjs.com/images/cards/halcyon.png"
                    height="125px"
                    contain
                  ></v-img>
                </v-flex>
              </v-layout>
              <v-divider light></v-divider>
              <v-btn
                color="white"
                dark
                small
                absolute
                left
                fab
              >
              <v-icon color="black">play_arrow</v-icon></v-btn>
              <v-card-actions class="pa-3">
                
                <v-spacer></v-spacer>
                <v-icon>star_border</v-icon>
                <v-icon>star_border</v-icon>
                <v-icon>star_border</v-icon>
                <v-icon>star_border</v-icon>
                <v-icon>star_border</v-icon>
              </v-card-actions>
            </v-card>
        </v-flex>
</template>

<script>
export default {

}
</script>

<style>

</style>
