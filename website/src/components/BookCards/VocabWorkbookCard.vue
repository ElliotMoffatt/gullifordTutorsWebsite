<template>
  <BookCard :imgSrc="imgSrc" :imgAlt="imgAlt" :title="title" :description="description" :review="review" :amazonLink="amazonLink">
    <template v-slot:cover>
      <img src="@/assets/covers/vocabWorkbookCover.png" :alt="imgAlt">
    </template>
  </BookCard>
</template>

<script>
import BookCard from '../BookCard.vue'
export default {
  name: 'VocabWorkbookCard',
  components: {
    BookCard
  },
  props: {
  },
  data () {
    return {
      imgSrc: '@/assets/covers/vocabWorkbookCover.png',
      imgAlt: 'Vocab Workbook Cover',
      title: 'My 11+ Vocabulary Workbook',
      description: null,
      review: 'Very useful to learn new words, but also to add your own new words, all in one place.',
      amazonLink: 'https://www.amazon.co.uk/gp/product/1694558126'
    }
  }
}
</script>
