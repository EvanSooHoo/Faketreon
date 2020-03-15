<template>

  
  <div class="faketreon">
    
    <v-app-bar
      color="white"
      dense
      light
    >
      <v-btn icon href="https://twitter.com/hashtag/faketreon?src=hash">
        <v-icon>mdi-alpha-f-circle</v-icon>
      </v-btn>

      <v-spacer></v-spacer>

      <v-btn icon>
        <v-icon>mdi-magnify</v-icon>
      </v-btn>
      <v-form>
        <v-container>
            <v-row>
              <v-col cols="12" sm="12">
                    <v-text-field
                >Search for a user</v-text-field>
              </v-col>
            </v-row>
        </v-container>
      </v-form>  
      <v-btn text small>Create on Patreon</v-btn>
      <v-btn text small>Log in</v-btn>
    </v-app-bar>

    <v-container fluid>
    <v-row justify="space-around">
      <v-col cols="12">
        
        <v-img src="https://i.picsum.photos/id/0/5616/3744.jpg" aspect-ratio="2.9"></v-img>
        <v-card flat tile class="d-flex">
          <v-row justify="space-around">
              
        </v-row>
        
        </v-card>
      </v-col>
      </v-row>
      </v-container>
      <v-row justify="space-around">
        <v-col cols="12">
        <v-avatar color="indigo" size="100">
          <span class="white--text headline"><v-img src="https://i.picsum.photos/id/166/200/300.jpg" position='center'></v-img></span> 
          <!--<span class="white--text headline">36</span>-->
        </v-avatar>
        </v-col>
        </v-row>
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
