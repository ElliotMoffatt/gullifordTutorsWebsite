<template>
  <BookCard :imgSrc="imgSrc" :imgAlt="imgAlt" :title="title" :description="description" :review="review" :amazonLink="amazonLink">
    <template v-slot:cover>
      <img src="@/assets/covers/shuffledSentencesCover.png" :alt="imgAlt">
    </template>
  </BookCard>
</template>

<script>
import BookCard from '../BookCard.vue'
export default {
  name: 'ClozeBookCard',
  components: {
    BookCard
  },
  props: {
  },
  data () {
    return {
      imgSrc: '@/assets/covers/shuffledSentencesCover.png',
      imgAlt: 'Shuffled Sentences Cover',
      title: 'Shuffled Sentences Practice Book',
      description: null,
      review: 'My daughter has been working through the examples over the past few weeks. Having plenty of examples is proving valuable, as this is one skill where practice really makes all the difference.',
      amazonLink: 'https://www.amazon.co.uk/gp/product/1089544685'
    }
  }
}
</script>
