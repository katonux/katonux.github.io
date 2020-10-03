<template>
  <div class="SocialButtons">
    <v-tooltip v-for="item in items" :key="item.title" bottom>
      <template v-slot:activator="{ on, attrs }">
        <v-btn
          icon
          v-bind="attrs"
          link
          :href="item.url"
          target="_blank"
          v-on="on"
        >
          <v-icon>{{ item.icon }}</v-icon>
        </v-btn>
      </template>
      <span>{{ item.title }}</span>
    </v-tooltip>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  data: () => {
    return {
      items: [
        {
          title: 'GitHub',
          icon: 'mdi-github',
          url: 'https://github.com/katonux',
        },
        {
          title: 'Twitter',
          icon: 'mdi-twitter',
          url: 'https://twitter.com/katonux',
        },
        {
          title: 'Telegram',
          icon: 'mdi-telegram',
          url: 'https://telegram.me/katonux',
        },
        {
          title: 'Email',
          icon: 'mdi-email',
          url: 'mailto:kato-shota@outlook.jp',
        },
      ],
    }
  },
})
</script>
