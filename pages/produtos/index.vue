<template>
  <v-layout>
    <v-flex>
      <div class="text-xs-center">
         <h1 text-xs-center>Produtos</h1>
      </div>


    <v-container grid-list-md text-xs-center>
      <v-layout row wrap>
      <v-flex xs4 v-for="post of posts">
       <a @click="openPost(post.id)">
        <v-card>
          <v-card-media v-bind:src="image" height="200px">
          </v-card-media>
          <v-card-title primary-title>
            <div>
              <h4  class="text-grey text-md-center">{{post.title}}</h4>
            </div>
          </v-card-title>
        </v-card>
       </a>
      </v-flex>
      </v-layout>
    </v-container>

    </v-flex>
  </v-layout>
</template>


<script>
  import axios from 'axios';

  export default {
    data(){
      return {
        userId: '',
        posts: [],
        image: 'https://i2.wp.com/beebom.com/wp-content/uploads/2016/01/Reverse-Image-Search-Engines-Apps-And-Its-Uses-2016.jpg?resize=640%2C426'
      }
    },
    methods: {
        openPost(id){
          let postId = id;
         this.$router.push('/produtos/'+postId)
        }
    },

    created(){
      axios.get('https://jsonplaceholder.typicode.com/posts')
        .then((response) => {
          this.posts = response.data;
          console.log(this.users)
        })
        .catch(error => {
          console.log(error)
        })
    }

  }
</script>
