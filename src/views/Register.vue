<template>
  <v-app>
    <v-content>
      <v-container fluid fill-height>
        <v-layout align-center justify-center>
          <v-flex xs12 sm8 md4>
            <v-card class="elevation-12">
              <v-toolbar dark color="primary">
                <v-toolbar-title>Sign up</v-toolbar-title>
                <v-spacer></v-spacer>
              </v-toolbar>
              <v-card-text>
                <v-form>
                  <v-text-field prepend-icon="person" v-model="username" label="Username" type="text"></v-text-field>
                  <v-text-field prepend-icon="person" v-model="email" label="Email" type="text"></v-text-field>
                  <v-text-field prepend-icon="lock" v-model="password" label="Password" id="password" type="password"></v-text-field>
                  <v-text-field prepend-icon="lock" v-model="password_confirmation" label="Confirm password" id="password_confirmation" type="password"></v-text-field>
                </v-form>
                Already have account? <router-link to="login" style="text-decoration: unset">Sign In</router-link>
              </v-card-text>
              <v-card-actions>
                <v-spacer></v-spacer>
                <v-btn color="primary">Sign up</v-btn>
              </v-card-actions>
            </v-card>
          </v-flex>
        </v-layout>
      </v-container>
    </v-content>
  </v-app>
</template>

<script>
export default {
  data() {
    return {
      form: {
        username: "",
        email: "",
        password: "",
        password_confirmation: "",
      }
    };
  }
};
</script>

<style>
</style>