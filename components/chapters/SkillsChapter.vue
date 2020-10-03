<template>
  <div class="SkillsChapter">
    <div class="mt-8 text-center">
      <h2>Skills</h2>
    </div>
    <v-container>
      <v-row justify="center">
        <v-col v-for="item in items" :key="item.title" class="py-5" md="2">
          <SkillCard
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
          imgClass: 'yellow lighten-3',
        },
        {
          title: 'HTML5',
          desc: 'Markup',
          iconName: 'fab fa-html5',
          imgClass: 'green lighten-1',
        },
        {
          title: 'JavaScript',
          desc: 'Language',
          iconName: 'mdi-language-javascript',
          imgClass: 'green lighten-1',
        },
        {
          title: 'TypeScript',
          desc: 'Frontend Framework',
          iconName: 'mdi-language-typescript',
          imgClass: 'green lighten-1',
        },
        {
          title: 'Vue.js',
          desc: 'Frontend Framework',
          iconName: 'fab fa-vuejs',
          imgClass: 'green lighten-1',
        },
        {
          title: 'Nuxt.js',
          desc: 'Markup',
          iconName: 'mdi-nuxt',
          imgClass: 'green lighten-1',
        },
        {
          title: 'Node.js',
          desc: 'Markup',
          iconName: 'mdi-nodejs',
          imgClass: 'green lighten-1',
        },
        {
          title: 'Angular',
          desc: 'Markup',
          iconName: 'fab fa-angular',
          imgClass: 'green lighten-1',
        },
        {
          title: 'Docker',
          desc: 'Containers Platform',
          iconName: 'fab fa-docker',
          imgClass: 'blue lighten-1',
        },
        {
          title: 'Python',
          desc: 'Containers Platform',
          iconName: 'fab fa-python',
          imgClass: 'blue lighten-1',
        },
        {
          title: 'Django',
          desc: 'Containers Platform',
          iconName: 'fab fa-python',
          imgClass: 'blue lighten-1',
        },
        {
          title: 'Git',
          desc: 'Containers Platform',
          iconName: 'mdi-git',
          imgClass: 'blue lighten-1',
        },
        {
          title: 'Vuetify',
          desc: 'Containers Platform',
          iconName: 'mdi-vuetify',
          imgClass: 'blue lighten-1',
        },
        {
          title: 'Bootstrap',
          desc: 'Containers Platform',
          iconName: 'mdi-bootstrap',
          imgClass: 'blue lighten-1',
        },
        {
          title: 'Swift',
          desc: 'Containers Platform',
          iconName: 'mdi-language-swift',
          imgClass: 'blue lighten-1',
        },
      ],
    }
  },
})
</script>
