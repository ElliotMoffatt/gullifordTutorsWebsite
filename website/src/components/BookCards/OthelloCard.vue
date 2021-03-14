<template>
  <BookCard :imgSrc="imgSrc" :imgAlt="imgAlt" :title="title" :description="description" :review="review" :amazonLink="amazonLink">
    <template v-slot:cover>
      <img src="@/assets/covers/OthelloCover.png" :alt="imgAlt">
    </template>
  </BookCard>
</template>

<script>
import BookCard from '../BookCard.vue'
export default {
  name: 'OthelloCard',
  components: {
    BookCard
  },
  props: {
  },
  data () {
    return {
      imgSrc: '@/assets/covers/OthelloCover.png',
      imgAlt: 'Othello Cover',
      title: '"Othello" guided GCSE revision notebook',
      description: null,
      review: "This book is brilliant. My daughter finds it hard to know how to create revision notes and how to organise them. It's been created in such a way that it would help any student whether aiming for a level 4 or 9. I'm amazed the schools don't use it.",
      amazonLink: 'https://www.amazon.co.uk/gp/product/1090532385'
    }
  }
}
</script>
