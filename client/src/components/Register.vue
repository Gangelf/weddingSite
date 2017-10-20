<template>
  <div>
    <v-app>
      <v-layout column>
        <v-flex xs6 offset-xs3>
          <div class="white elevation-2">
            <v-toolbar flat dense class="cyan" dark>
              <v-toolbar-title>Register</v-toolbar-title>
            </v-toolbar>
            <div class="pl-4 pr-4 pt-2 pb-2">
              <v-text-field type="email" name="email" placeholder="email" v-model="email"></v-text-field>
              <br>
              <v-text-field type="password" name="password" placeholder="password" v-model="password"></v-text-field>
              <br>
              <v-btn @click="register" class="cyan" dark>Register</v-btn>
            </div>
          </div>
        </v-flex>
      </v-layout>
    </v-app>
  </div>
</template>

<script>
  import AuthenticationService from '@/services/AuthenticationService'
  export default {
    data () {
      return {
        email: '',
        password: ''
      }
    },
    methods: {
      async register () {
        const response = await AuthenticationService.register({
          email: this.email,
          password: this.password
        })
        console.log(response.data)
      }
    }

  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
