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
              <div class="text-center">
                <v-btn
                  rounded
                  color="primary"
                  dark
                  @click="snackbarOne = true"
                >
                  Donate
                </v-btn>
                <v-snackbar
                  v-model="snackbarOne"
                  :multi-line="multiLine"
                >
                  {{ calmText }}
                  <v-btn
                    color="green"
                    text
                    @click="snackbarOne = false"
                  >
                    Close
                  </v-btn>
                </v-snackbar>
              </div>
                  
                

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
                <v-btn
                  rounded
                  color="primary"
                  dark
                  @click="snackbarTwo = true"
                >
                  Donate
                </v-btn>
                <v-snackbar
                  v-model="snackbarTwo"
                  :multi-line="multiLine"
                >
                  {{ weirdText }}
                  <v-btn
                    color="orange"
                    text
                    @click="snackbarTwo = false"
                  >
                    Close
                  </v-btn>
                </v-snackbar>
              </div>
                <ul>
                  <li>Bullet point</li>
                  <li>Bullet point</li>
                  <li>Bullet point</li>
                </ul>
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
                <v-btn
                  rounded
                  color="primary"
                  dark
                  @click="snackbarThree = true"
                >
                  Donate
                </v-btn>
                <v-snackbar
                  v-model="snackbarThree"
                  :multi-line="multiLine"
                >
                  {{ angryText }}
                  <v-btn
                    color="red"
                    text
                    @click="snackbarThree = false"
                  >
                    Close
                  </v-btn>
                </v-snackbar>
              </div>
              <ul>
                <li>Bullet point</li>
                <li>Bullet point</li>
                <li>Bullet point</li>
              </ul>    
              
            </v-card>
            
          </v-col>
        </v-row>
  </v-container>
  </div>
</template>

<script>
export default {
  data () {
      return {
        dialog: false,
        multiLine: false,
      snackbarOne: false,
      snackbarTwo: false,
      snackbarThree: false,
      calmText: 'You can\'t actually donate, but thank you!',
      weirdText: 'You can\'t actually donate, and do you know how often I post?',
      angryText: 'DONATING IS ACTUALLY IMPOSSIBLE',
      }
    },
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
  margin: 20px 0 0;
  
  padding: 0;
  text-align: "left";
}
li {
  margin: 0;
  padding: 0;
  text-align: "left";
}
/*
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
*/
a {
  color: #42b983;
}
</style>
