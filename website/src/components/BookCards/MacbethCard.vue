<template>
  <BookCard :imgSrc="imgSrc" :imgAlt="imgAlt" :title="title" :description="description" :review="review" :amazonLink="amazonLink">
    <template v-slot:cover>
      <img src="@/assets/covers/macbethCover.png" :alt="imgAlt">
    </template>
  </BookCard>
</template>

<script>
import BookCard from '../BookCard.vue'
export default {
  name: 'MacbethCard',
  components: {
    BookCard
  },
  props: {
  },
  data () {
    return {
      imgSrc: '@/assets/covers/macbethCover.png',
      imgAlt: 'Macbeth Cover',
      title: '"Macbeth" guided GCSE revision notebook',
      description: null,
      review: 'Great revision guide!',
      amazonLink: 'https://www.amazon.co.uk/gp/product/1093225785'
    }
  }
}
</script>
