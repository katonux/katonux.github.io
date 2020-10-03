<template>
  <div class="SkillsChapter my-16">
    <div class="text-center">
      <h2>Skills</h2>
    </div>
    <v-container v-if="mobile" style="overflow-x: scroll; display: flex">
      <v-col v-for="item in items" :key="item.title">
        <skill-card
          :icon-name="item.iconName"
          :title="item.title"
          :desc="item.desc"
          :img-class="item.imgClass"
          :img-src="item.imgSrc"
          style="display: inline-block"
        />
      </v-col>
    </v-container>
    <v-container v-else style="max-width: 1200px">
      <v-row justify="start">
        <v-col
          v-for="item in items"
          :key="item.title"
          class="d-flex py-5 justify-center"
        >
          <skill-card
            :icon-name="item.iconName"
            :title="item.title"
            :desc="item.desc"
            :img-class="item.imgClass"
            :img-src="item.imgSrc"
          />
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import SkillCard from '@/components/molecules/SkillCard.vue'
export default Vue.extend({
  components: {
    SkillCard,
  },
  data: () => {
    return {
      items: [
        {
          title: 'Linux',
          desc: 'Operating System',
          iconName: 'fab fa-linux',
          imgClass: 'grey lighten-1',
        },
        {
          title: 'HTML5',
          desc: 'Markup Language',
          iconName: 'fab fa-html5',
          imgClass: 'red lighten-1',
        },
        {
          title: 'JavaScript',
          desc: 'Programming Language',
          iconName: 'mdi-language-javascript',
          imgClass: 'yellow lighten-1',
        },
        {
          title: 'TypeScript',
          desc: 'Programming Language',
          iconName: 'mdi-language-typescript',
          imgClass: 'blue lighten-1',
        },
        {
          title: 'Vue.js',
          desc: 'JavaScript Framework',
          iconName: 'fab fa-vuejs',
          imgClass: 'green',
        },
        {
          title: 'Nuxt.js',
          desc: 'JavaScript Framework',
          iconName: 'mdi-nuxt',
          imgClass: 'light-green lighten-3',
        },
        {
          title: 'Node.js',
          desc: 'JavaScript Runtime',
          iconName: 'mdi-nodejs',
          imgClass: 'light-green lighten-1',
        },
        {
          title: 'Angular',
          desc: 'Frontend Framework',
          iconName: 'fab fa-angular',
          imgClass: 'red lighten-3',
        },
        {
          title: 'Docker',
          desc: 'Containers Platform',
          iconName: 'fab fa-docker',
          imgClass: 'blue lighten-2',
        },
        {
          title: 'Python',
          desc: 'Programming Language',
          iconName: 'fab fa-python',
          imgClass: 'deep-purple lighten-2',
        },
        {
          title: 'Django',
          desc: 'Python Web Framework',
          iconName: 'fab fa-python',
          imgClass: 'teal lighten-1',
        },
        {
          title: 'Git',
          desc: 'Version Control System',
          iconName: 'mdi-git',
          imgClass: 'orange darken-1',
        },
        {
          title: 'Vuetify',
          desc: 'CSS Framework',
          iconName: 'mdi-vuetify',
          imgClass: 'light-blue lighten-3',
        },
        {
          title: 'Bootstrap',
          desc: 'CSS Framework',
          iconName: 'mdi-bootstrap',
          imgClass: 'indigo lighten-1',
        },
        {
          title: 'Swift',
          desc: 'Programming Language',
          iconName: 'mdi-language-swift',
          imgClass: 'orange lighten-2',
        },
      ],
    }
  },
  computed: {
    mobile(): Boolean {
      if (
        this.$vuetify.breakpoint.name === 'sm' ||
        this.$vuetify.breakpoint.name === 'xs'
      ) {
        return true
      } else {
        return false
      }
    },
  },
})
</script>
