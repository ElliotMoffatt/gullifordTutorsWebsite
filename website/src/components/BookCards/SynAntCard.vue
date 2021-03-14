<template>
  <BookCard :imgSrc="imgSrc" :imgAlt="imgAlt" :title="title" :description="description" :review="review" :amazonLink="amazonLink">
    <template v-slot:cover>
      <img src="@/assets/covers/synAndAntCover.png" :alt="imgAlt">
    </template>
  </BookCard>
</template>

<script>
import BookCard from '../BookCard.vue'
export default {
  name: 'SynAntBookCard',
  components: {
    BookCard
  },
  props: {
  },
  data () {
    return {
      imgSrc: '@/assets/covers/synAndAntCover.png',
      imgAlt: 'Synonyms and Antonyms Cover',
      title: 'Synonyms and Antonyms Missing Letters',
      description: null,
      review: 'My 10-year old started doing the tests in this book during lockdown. I am amazed at how much this has improved his vocab generally - new words seem to be popping up unexpectedly in his spoken English too which always surprises me!',
      amazonLink: 'https://www.amazon.co.uk/gp/product/1082205273'
    }
  }
}
</script>
