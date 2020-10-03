<template>
  <div>
    <BookCover />
    <SkillsChapter />
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import BookCover from '@/components/chapters/BookCover.vue'
import SkillsChapter from '@/components/chapters/SkillsChapter.vue'
export default Vue.extend({
  components: {
    BookCover,
    SkillsChapter,
  },
})
</script>
