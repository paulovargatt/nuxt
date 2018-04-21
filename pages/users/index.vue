<template>
  <v-layout>
    <p>Digite um user</p>
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
  }
</script>
