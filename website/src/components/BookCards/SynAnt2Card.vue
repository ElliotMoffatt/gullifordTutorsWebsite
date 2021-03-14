<template>
  <BookCard :imgSrc="imgSrc" :imgAlt="imgAlt" :title="title" :description="description" :review="review" :amazonLink="amazonLink">
    <template v-slot:cover>
      <img src="@/assets/covers/synAndAntMissingLettersBook2Cover.png" :alt="imgAlt">
    </template>
  </BookCard>
</template>

<script>
import BookCard from '../BookCard.vue'
export default {
  name: 'SynAntBook2Card',
  components: {
    BookCard
  },
  props: {
  },
  data () {
    return {
      imgSrc: '@/assets/covers/synAndAntMissingLettersBook2Cover.png',
      imgAlt: 'Synonyms and Antonyms Book 2 Cover',
      title: 'Synonyms and Antonyms Missing Letters: Book 2',
      description: null,
      review: 'Fab book, easy to use for both myself and my daughter, highly recommend.',
      amazonLink: 'https://www.amazon.co.uk/gp/product/B087SGBBZB'
    }
  }
}
</script>
