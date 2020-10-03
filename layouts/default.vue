<template>
  <v-app dark>
    <v-main class="grey darken-3">
      <!-- <v-navigation-drawer
        class="ma-8 elevation-16 rounded-xl"
        height="400"
        elevation
        permanent
        style="position: absolute; top: 0; left: 0; z-index: 10"
      >
        <v-list rounded>
          <v-list-item link>
            <v-list-item-icon>
              <v-icon>mdi-arrow-up-bold</v-icon>
            </v-list-item-icon>
            <v-list-item-content>
              <v-list-item-title>TOP</v-list-item-title>
            </v-list-item-content>
          </v-list-item>
          <v-list-item link>
            <v-list-item-icon>
              <v-icon>mdi-xml</v-icon>
            </v-list-item-icon>
            <v-list-item-content>
              <v-list-item-title>Skills</v-list-item-title>
            </v-list-item-content>
          </v-list-item>
          <v-list-item link>
            <v-list-item-icon>
              <v-icon>mdi-cube-outline</v-icon>
            </v-list-item-icon>
            <v-list-item-content>
              <v-list-item-title>Works</v-list-item-title>
            </v-list-item-content>
          </v-list-item>
        </v-list>
      </v-navigation-drawer> -->
      <nuxt />
    </v-main>
    <v-footer>
      <span>&copy; {{ new Date().getFullYear() }}</span>
    </v-footer>
  </v-app>
</template>
