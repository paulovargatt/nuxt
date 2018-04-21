<template>
  <v-app light>
    <v-toolbar app>
        <v-icon @click="back()" class="back_button chevron_right" v-html="'chevron_left'"></v-icon>
      <v-toolbar-title v-text="title"></v-toolbar-title>
      <v-spacer></v-spacer>

    </v-toolbar>
    <v-content>
      <v-container>
        <nuxt />
      </v-container>
    </v-content>

    <v-footer app>
      <span>&copy; 2035</span>
    </v-footer>
  </v-app>
</template>

<style>
  .back_button{
    cursor: pointer;
  }
</style>

<script>
  export default {
    data() {
      return {
        title: 'USERS Section'
      }
    },
      methods: {
          back(){
              window.history.back();
          }
      }
  }
</script>

<style>
  #app > div > nav > div > button:nth-child(7){
    display: none;
  }
</style>
