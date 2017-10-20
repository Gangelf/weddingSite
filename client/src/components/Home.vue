<template>
  <div>
    <v-app>
      <v-layout column>
        <v-flex>
          <v-toolbar fixed class="purple darken-1" dark>
            <v-toolbar-title >A&S</v-toolbar-title>
            <v-spacer></v-spacer>
            <v-toolbar-side-icon class="hidden-md-and-up"></v-toolbar-side-icon>
            <v-toolbar-side class="hidden-sm-and-down">
              <v-btn flat>About Us</v-btn>
              <v-btn flat>R.S.V.P</v-btn>
              <v-btn flat>Venue/Hotel Information</v-btn>
              <v-btn flat>Registry</v-btn>
              <v-btn flat>Music Request</v-btn>
            </v-toolbar-side>
          </v-toolbar>
        </v-flex>
      </v-layout>
    </v-app>
  </div>
</template>

<script>
  export default {
    data () {
      return {
      }
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
