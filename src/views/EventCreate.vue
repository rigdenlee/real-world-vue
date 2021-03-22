<template>
  <div class="about">
    <h1>Create Event, {{user.id }}</h1>
    <!-- <p>This event was created by {{ user.id }}</p> -->
    <!-- <ul> -->
      <!-- <li v-for="cat in categories" :key="cat">{{ cat }}</li> -->
    <!-- </ul> -->
  </div>
</template>

<script>
  import { mapState } from 'vuex';

  export default {
    computed: mapState([ 
      'user'
      // categories: 'categories'
    ])
      // userName() {
      //   return this.$store.state.user.name
      // },
      // userID() {
      //   return this.$store.state.user.id
      // }
    
  }
</script>

<style scoped>

</style>