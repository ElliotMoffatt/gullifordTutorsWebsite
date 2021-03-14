<template>
  <div class="card m-1 mb-3 container" style="max-width: 600px; display:inline-block">
    <div class="row g-0">
      <div class="col col-auto imgHolder">
        <slot name="cover"></slot>
      </div>
      <div class="col col-8">
        <div class="card-body">
          <h5 class="card-title">{{title}}</h5>
          <p class="card-text">{{description}}</p>
          <p class="card-text"><i>"{{review}}"</i></p>
          <p class="card-text"><small class="text-muted"><GetItOnAmazon :link="amazonLink"></GetItOnAmazon></small></p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import GetItOnAmazon from './GetItOnAmazon.vue'
export default {
  name: 'BookCard',
  components: {
    GetItOnAmazon
  },
  props: {
    title: String,
    description: String,
    review: String,
    amazonLink: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .imgHolder img {
    max-height: 200px;
    max-width: 170px;
  }
</style>
