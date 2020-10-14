<template>
  <div
    class="WorksChapter py-16"
    style="background-image: linear-gradient(-90deg, #85a333, #0db0c9)"
  >
    <div class="text-center">
      <h2>Works</h2>
    </div>
    <v-container>
      <v-row>
        <v-col class="d-flex justify-center" cols="12">
          <v-card width="700px">
            <v-img src="/nemushee_header.png" />
            <v-card-title>Nemushee.net</v-card-title>
            <v-card-text> Self-hosted mastodon instance </v-card-text>
          </v-card>
        </v-col>
        <v-col class="d-flex justify-center" cols="12">
          <v-card width="700px">
            <v-img class="grey lighten-2">
              <v-row align="center" justify="center" style="height: 280px">
                <v-col class="align-center text-center" cols="12">
                  <v-avatar size="100" class="my-4">
                    <img
                      src="https://avatars0.githubusercontent.com/u/36836040?s=460&u=b80acba5bc20a660cb0c4edbfa042b6431fc3f2a&v=4"
                      alt="katonux"
                    />
                  </v-avatar>
                </v-col>
              </v-row>
            </v-img>
            <v-card-title>katonux.github.io</v-card-title>
            <v-card-text>
              This Page! I used Nuxt.js generate and Vuetify.
            </v-card-text>
          </v-card>
        </v-col>
        <v-col class="d-flex justify-center" cols="12">
          <v-card width="700px">
            <v-img class="orange lighten-1">
              <v-row align="center" justify="center" style="height: 280px">
                <v-col class="align-center text-center" cols="3">
                  <v-icon size="100">mdi-spotify</v-icon>
                </v-col>
                <v-col class="align-center text-center" cols="3">
                  <v-icon size="100">mdi-twitter</v-icon>
                </v-col>
              </v-row>
            </v-img>
            <v-card-title>Spotify Nowplaying</v-card-title>
            <v-card-text>
              Post the track playing on Spotify to Twitter.
            </v-card-text>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>
