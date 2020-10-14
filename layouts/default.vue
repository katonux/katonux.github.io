<template>
  <v-app dark>
    <v-main class="grey darken-2">
      <nuxt />
    </v-main>
    <v-footer>
      <span>&copy; {{ new Date().getFullYear() }}</span>
      <v-spacer />
      <privacy-policy />
    </v-footer>
  </v-app>
</template>

<script lang="ts">
import Vue from 'vue'
import PrivacyPolicy from '@/components/molecules/PrivacyPolicy.vue'
export default Vue.extend({
  components: {
    PrivacyPolicy,
  },
})
</script>
