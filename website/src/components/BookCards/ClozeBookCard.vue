<template>
  <BookCard :imgSrc="imgSrc" :imgAlt="imgAlt" :title="title" :description="description" :review="review" :amazonLink="amazonLink">
    <template v-slot:cover>
      <img src="@/assets/covers/clozeCover.png" :alt="imgAlt">
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
      imgSrc: '@/assets/covers/clozeCover.png',
      imgAlt: 'Cloze Book Cover',
      title: 'Cloze Practice Book',
      description: null,
      review: "I've bought various tutor books over the last couple of years, but really like how clearly this is set out, one of my favorites",
      amazonLink: 'https://www.amazon.co.uk/gp/product/1708457194'
    }
  }
}
</script>
