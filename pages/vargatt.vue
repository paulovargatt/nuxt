<template>
  <v-layout>
    <v-flex text-xs-center>
      <blockquote class="blockquote">
       {{title}} é foda
       {{myObg.title}} é foda
        <footer>
        </footer>
      </blockquote>
    </v-flex>
  </v-layout>
</template>


<script>
  export default {
    data(){
      return {
        title: 'Vargatt',

        myObg: {
          title: 'number',
          desc: 'teste'
        }
      }
    }

  }
</script>
