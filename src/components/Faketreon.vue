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
        <v-row>
          <v-col cols="12">
            <center><b>Evan</b></center>
            <center>is creating blog posts, long Facebook statuses, and fake Patreon pages</center>
            <br>
            <br>
            <h3>Select a membership level</h3>
            <center></center>
          </v-col>
        </v-row>
      <v-container class="grey lighten-5">
        <v-row no-gutters>
          <v-col order="last">
            <v-card
              class="pa-2"
              outlined
              tile
            >
              <h4>Thank you for your support!</h4>
              <br>
              <br>
              <h1>
                $1 per post 
              </h1>
              <br>
              
              <v-dialog v-model="dialog" persistent max-width="600px">
                <div class="text-center">
                  </div>
                  <template v-slot:activator="{ on }">
                    <v-btn rounded color="primary" v-on="on" dark>Donate</v-btn>
                  </template>
                  <v-card>
                    <v-card-title class="headline">Use Google's location service?</v-card-title>
                    <v-card-text>Let Google help apps determine location. This means sending anonymous location data to Google, even when no apps are running.</v-card-text>
                    <v-card-actions>
                      <v-spacer></v-spacer>
                      <v-btn color="green darken-1" text @click="dialog = false">Disagree</v-btn>
                      <v-btn color="green darken-1" text @click="dialog = false">Agree</v-btn>
                    </v-card-actions>
                  </v-card>
                
                </v-dialog>
            </v-card>
          </v-col>
          <v-col>
            <v-card
              class="pa-2"
              outlined
              tile
            >
              <h4>Thank you for even more support!</h4>
              <br>
              <br>
              <h1>
                $5 per post 
              </h1>
              <br>
              <div class="text-center">
                  <v-btn rounded color="primary" dark>Donate</v-btn>
                </div>
            </v-card>
          </v-col>
          <v-col order="first">
            <v-card
              class="pa-2"
              outlined
              tile
            >
              <h4>That's way too much what are you doing</h4>
              <br>
              <br>
              <h1>
                $20 per post 
              </h1>
              <br>
              <div class="text-center">
                <v-btn rounded color="primary" dark>Donate</v-btn>
              </div>
            </v-card>
            
          </v-col>
        </v-row>
  </v-container>
  </div>
</template>

<script>
export default {
  dialog: true,
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

h4 {
  margin: 20px 0 0;
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
