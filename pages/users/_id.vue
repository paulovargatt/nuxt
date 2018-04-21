<template>
  <v-layout>
    <v-flex text-xs-center>
      <blockquote class="blockquote">
        <h1>USER X {{$route.params.id}}</h1>
        <footer>
        </footer>
      </blockquote>
    </v-flex>
  </v-layout>
</template>

<script>
  export default {
      validate(data){
          console.log(data);
          return true
      }
  }
</script>