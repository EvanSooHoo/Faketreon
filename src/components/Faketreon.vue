<template>

  
  <div class="faketreon">
    <v-card
    color="grey lighten-4"
    flat
    height="200px"
    tile
  >
    <v-toolbar dense>
      

      

      <v-btn icon>
        <v-icon>mdi-magnify</v-icon>
      </v-btn>

      
    </v-toolbar>
  </v-card>
    
  </div>
</template>

<script>
export default {
  name: 'Faketreon',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
