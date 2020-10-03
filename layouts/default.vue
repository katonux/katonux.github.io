<template>
  <v-app dark>
    <v-app-bar fixed app dense>
      <v-toolbar-title v-text="title" />
    </v-app-bar>
    <v-main>
      <nuxt />
    </v-main>
    <v-footer :absolute="!fixed" app>
      <span>&copy; {{ new Date().getFullYear() }}</span>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  data() {
    return {
      title: 'KATONUX',
    }
  },
}
</script>
