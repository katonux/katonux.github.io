<template>
  <v-app dark>
    <v-app-bar fixed app dense>
      <v-toolbar-title />
    </v-app-bar>
    <v-main class="grey darken-3">
      <nuxt />
    </v-main>
    <v-footer app>
      <span>&copy; {{ new Date().getFullYear() }}</span>
    </v-footer>
  </v-app>
</template>
