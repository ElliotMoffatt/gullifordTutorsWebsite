<template>
  <div class="home">

    <h3>Popular right now:</h3>
    <ShuffledSentencesCard></ShuffledSentencesCard>
    <SynAntCard></SynAntCard>

  </div>
</template>

<script>
// @ is an alias to /src
import ShuffledSentencesCard from '@/components/BookCards/ShuffledSentencesCard.vue'
import SynAntCard from '@/components/BookCards/SynAntCard.vue'

export default {
  name: 'Home',
  components: {
    ShuffledSentencesCard,
    SynAntCard
  }
}
</script>
