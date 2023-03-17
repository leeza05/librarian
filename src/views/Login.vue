<template>
    <div class="centre">
      <v-row>
        <v-col col="10" sm="6" offset-sm="3" md="4" offset-md="4" offset="1">
            <v-avatar size="95" tile>
                <v-img src="@/assets/logo.png"></v-img>
            </v-avatar>
            <v-text-field label="Username" v-model="Username"></v-text-field>
            <v-text-field label="Password" type="password" v-model="Password"></v-text-field>
            <v-btn block elevation="2" @click="authenticate()">Login</v-btn>
        </v-col>
      </v-row>
    </div>
  </template>
  
  <script>
  
    export default {
        data() {
            return {
                Username: '',
                Password: ''
            }
        },
        methods(){
            authenticate()
        }
    }
  </script>