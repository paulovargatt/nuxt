<template>
  <v-layout>
    <v-flex text-xs-center>
         <h1>Users Aki</h1>
        <input class="blue-grey text--white" type="text" v-model="userId" />
        <button @click="onLoadUser()" class="btn btn--small">Carregar</button>
        <nuxt-child />
    </v-flex>
  </v-layout>
</template>


<script>
  export default {
    data(){
      return {
        userId: ''
      }
    },
    methods: {
        onLoadUser(){
          this.$router.push('/users/'+ this.userId)
        }
    },
      layout: 'users'
  }
</script>
