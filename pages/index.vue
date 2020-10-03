<template>
  <div>
    <BookCover />
    <SkillsChapter />
    <works-chapter />
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import BookCover from '@/components/chapters/BookCover.vue'
import SkillsChapter from '@/components/chapters/SkillsChapter.vue'
import WorksChapter from '@/components/chapters/WorksChapter.vue'
export default Vue.extend({
  components: {
    BookCover,
    SkillsChapter,
    WorksChapter,
  },
})
</script>
