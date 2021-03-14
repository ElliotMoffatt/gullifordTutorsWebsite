<template>
  <BookCard :imgSrc="imgSrc" :imgAlt="imgAlt" :title="title" :description="description" :review="review" :amazonLink="amazonLink">
    <template v-slot:cover>
      <img src="@/assets/covers/inspectorCallsCover.png" :alt="imgAlt">
    </template>
  </BookCard>
</template>

<script>
import BookCard from '../BookCard.vue'
export default {
  name: 'InspectorCallsCard',
  components: {
    BookCard
  },
  props: {
  },
  data () {
    return {
      imgSrc: '@/assets/covers/inspectorCallsCover.png',
      imgAlt: 'An Inspector Calls Cover',
      title: '"An Inspector Calls" guided GCSE revision notebook',
      description: null,
      review: 'The book has well set out essay pages to use covering all the main revision topics needed. A great learning tool! I would highly recommend as a GCSE revision guide.',
      amazonLink: 'https://www.amazon.co.uk/gp/product/1795708891'
    }
  }
}
</script>
