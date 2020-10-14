<template>
  <div>
    <book-cover />
    <skills-chapter />
    <works-chapter />
    <profile-chapter />
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import BookCover from '@/components/chapters/BookCover.vue'
import SkillsChapter from '@/components/chapters/SkillsChapter.vue'
import WorksChapter from '@/components/chapters/WorksChapter.vue'
import ProfileChapter from '@/components/chapters/ProfileChapter.vue'
export default Vue.extend({
  components: {
    BookCover,
    SkillsChapter,
    WorksChapter,
    ProfileChapter,
  },
})
</script>
