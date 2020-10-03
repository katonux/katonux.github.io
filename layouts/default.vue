<template>
  <v-app dark>
    <v-app-bar fixed app dense>
      <v-toolbar-title v-text="title" />
    </v-app-bar>
    <v-main class="grey darken-3">
      <NavigationDrawer />
      <nuxt />
    </v-main>
    <v-footer app>
      <span>&copy; {{ new Date().getFullYear() }}</span>
    </v-footer>
  </v-app>
</template>

<script lang="ts">
import Vue from 'vue'
import NavigationDrawer from '@/components/NavigationDrawer.vue'
export default Vue.extend({
  components: {
    NavigationDrawer,
  },
  data() {
    return {
      title: 'KATONUX',
      items: [
        { title: 'Home', icon: 'mdi-view-dashboard' },
        { title: 'About', icon: 'mdi-forum' },
      ],
    }
  },
})
</script>
