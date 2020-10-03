<template>
  <v-app dark>
    <v-app-bar fixed app dense>
      <v-toolbar-title v-text="title" />
    </v-app-bar>
    <v-main>
      <v-navigation-drawer
        floating
        permanent
        absolute
        class="ma-10"
        height="200"
      >
        <v-list dense rounded>
          <v-list-item link>
            <v-list-item-icon>
              <v-icon>mdi-check</v-icon>
            </v-list-item-icon>
          </v-list-item>
        </v-list>
      </v-navigation-drawer>
      <nuxt />
    </v-main>
    <v-footer app>
      <span>&copy; {{ new Date().getFullYear() }}</span>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  data() {
    return {
      title: 'KATONUX',
      items: [
        { title: 'Home', icon: 'mdi-view-dashboard' },
        { title: 'About', icon: 'mdi-forum' },
      ],
    }
  },
}
</script>
