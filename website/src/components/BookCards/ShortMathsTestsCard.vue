<template>
  <BookCard :imgSrc="imgSrc" :imgAlt="imgAlt" :title="title" :description="description" :review="review" :amazonLink="amazonLink">
    <template v-slot:cover>
      <img src="@/assets/covers/shortMathsTestsCover.png" :alt="imgAlt">
    </template>
  </BookCard>
</template>

<script>
import BookCard from '../BookCard.vue'
export default {
  name: 'ShortMathsTestsCard',
  components: {
    BookCard
  },
  props: {
  },
  data () {
    return {
      imgSrc: '@/assets/covers/shortMathsTestsCover.png',
      imgAlt: 'Short Maths Tests Cover',
      title: 'Short Maths Tests',
      description: null,
      review: 'Excellent book presenting bite-sized, clear maths tests that work on both speed and accuracy. The 12 minute format makes them a realistic daily achievement in the run up to 11 plus exam.',
      amazonLink: 'https://www.amazon.co.uk/gp/product/B08G9X15MM'
    }
  }
}
</script>
