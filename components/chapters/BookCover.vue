<template>
  <div class="BookCover">
    <v-container
      fluid
    >
      <v-row align="center" justify="center" style="height: 100vh">
        <v-col class="text-center" cols="12">
          <client-only>
            <v-avatar size="150" class="my-4">
              <img
                src="https://avatars0.githubusercontent.com/u/36836040?s=460&u=b80acba5bc20a660cb0c4edbfa042b6431fc3f2a&v=4"
                alt="katonux"
              />
            </v-avatar>
            <h1 class="display-1 font-weight-thin mb-4">Katonux</h1>
            <h4 class="subheading">Shota Kato</h4>
            <div class="mt-3">
              <social-buttons />
            </div>
            <v-col slot="placeholder" cols="12">
              <v-progress-circular
                indeterminate
                size="50"
                color="white"
              ></v-progress-circular>
            </v-col>
          </client-only>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import SocialButtons from '@/components/molecules/SocialButtons.vue'
export default Vue.extend({
  components: {
    SocialButtons,
  },
})
</script>
