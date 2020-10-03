<template>
  <div class="SkillsChapter">
    <div class="mt-8 text-center">
      <h2>Skills</h2>
    </div>

    <v-container>
      <v-row justify="center">
        <v-col v-for="n in 12" :key="n" class="py-5" md="2">
          <v-card width="200">
            <v-img class="yellow lighten-3" height="180px">
              <v-container fluid fill-height>
                <v-row align="center" justify="center">
                  <v-col class="text-center" cols="12">
                    <v-icon color="black" size="100">fab fa-linux</v-icon>
                  </v-col>
                </v-row>
              </v-container>
            </v-img>
            <v-card-title>Linux</v-card-title>
            <v-card-subtitle>Operating System</v-card-subtitle>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>
