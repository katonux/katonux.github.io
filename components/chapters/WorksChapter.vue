<template>
  <div
    class="WorksChapter py-16"
  >
    <div class="text-center">
      <h2>Works</h2>
    </div>
    <v-container>
      <v-row>
        <v-col class="d-flex justify-center" cols="12">
          <v-card
            hover
            href="https://nemushee.net"
            target="_blank"
            rounded="lg"
            light
            width="600px"
          >
            <v-img src="/nemushee_lemon.png" />
            <v-card-title>Nemushee.net</v-card-title>
            <v-card-text>
              オープンソースのミニブログ・分散型SNSサービス「Mastodon」のインスタンスです。自宅にインフラを構築して運営しています。
            </v-card-text>
          </v-card>
        </v-col>
        <v-col class="d-flex justify-center" cols="12">
          <v-card
            hover
            href="https://spotify-nowplaying.web.app"
            target="_blank"
            rounded="lg"
            light
            width="600px"
          >
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
              Spotifyで再生中の曲をTwitterに投稿できるやつです。
            </v-card-text>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>
