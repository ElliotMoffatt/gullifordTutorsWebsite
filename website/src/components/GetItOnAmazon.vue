<template>
  <a v-bind:href="link"
     target="_blank"
     rel="noopener noreferrer">
    Get it on Amazon.co.uk
    <i class="bi bi-arrow-up-right-square ml-1"></i>
  </a>
</template>

<script>export default {
  name: 'GetItOnAmazon',
  props: {
    link: String
  }
}</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  h3 {
    margin: 40px 0 0;
  }

  ul {
    list-style-type: none;
    padding: 0;
  }

  li {
    display: inline-block;
    margin: 0 10px;
  }

  a {
    color: #42b983;
  }
</style>
