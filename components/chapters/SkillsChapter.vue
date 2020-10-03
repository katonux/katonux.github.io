<template>
  <div class="SkillsChapter">
    <div class="mt-8 text-center">
      <h2>Skills</h2>
    </div>
    <v-container style="max-width: 1300px">
      <v-row justify="center">
        <v-col
          v-for="item in items"
          :key="item.title"
          class="d-flex py-5 justify-center"
        >
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
          imgClass: 'green',
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
          imgClass: 'red lighten-1',
        },
        {
          title: 'Docker',
          desc: 'Containers Platform',
          iconName: 'fab fa-docker',
          imgClass: 'blue lighten-1',
        },
        {
          title: 'Python',
          desc: 'Programming Language',
          iconName: 'fab fa-python',
          imgClass: 'deep-purple lighten-1',
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
})
</script>
