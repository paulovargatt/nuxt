<template>
  <v-layout>
    <v-flex text-xs-center>
      <blockquote class="blockquote">
        <h1>{{post.title}}</h1>
        <p>{{post.body}}</p>
        <footer>
        </footer>
      </blockquote>
    </v-flex>
  </v-layout>
</template>

<script>

  import axios from 'axios';

  export default {
    validate(data){
      return /^\d+$/.test(data.params.id)//TESTA ROTA Possui letras
    },

    data(){
      return {
        post: [],
      }
    },


    beforeCreate(){
      let id = this.$route.params.id;
        axios.get('https://jsonplaceholder.typicode.com/posts/'+id)
          .then((result => {
            this.post = result.data;
            console.log(this.post)
          }))
    }
  }


</script>
