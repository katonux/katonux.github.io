<template>
  <div class="SkillCard">
    <v-card width="200" class="rounded-lg">
      <v-img :class="imgClass" height="180px">
        <v-container fluid fill-height>
          <v-row align="center" justify="center">
            <v-col class="text-center" cols="12">
              <v-icon color="black" size="100" v-text="iconName"></v-icon>
            </v-col>
          </v-row>
        </v-container>
      </v-img>
      <v-card-title>{{ title }}</v-card-title>
      <v-card-subtitle>{{ desc }}</v-card-subtitle>
    </v-card>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  props: {
    title: {
      type: String,
      default: '',
    },
    desc: {
      type: String,
      default: '',
    },
    imgClass: {
      type: String,
      default: '',
    },
    iconName: {
      type: String,
      default: '',
    },
  },
})
</script>
