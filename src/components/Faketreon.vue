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
