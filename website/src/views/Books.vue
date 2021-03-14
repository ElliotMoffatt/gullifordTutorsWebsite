<template>
  <div id="books" class="books row">

    <nav id="books-navbar" class="navbar navbar-light bg-light col-2" style="align-content:start;position:sticky;top:20px;overflow:hidden; height:min-content">
      <nav class="nav nav-pills flex-column">
        <a class="nav-link groupTitle" href="#11Plus"><h4>11+ workbooks</h4></a>
        <nav class="nav nav-pills flex-column">
          <a class="nav-link ml-3 mt-1" href="#cloze">Cloze</a>
          <a class="nav-link ml-3 my-1" href="#vocab">Vocab Workbook</a>
          <a class="nav-link ml-3 my-1" href="#maths">Short Maths Tests</a>
          <a class="nav-link ml-3 my-1" href="#shuffled">Shuffled Sentences</a>
          <a class="nav-link ml-3 my-1" href="#synAnt">Synonyms and Antonyms Book 1</a>
          <a class="nav-link ml-3 my-1" href="#synAnt2">Synonyms and Antonyms Book 2</a>
        </nav>
        <a class="nav-link groupTitle" href="#revisionGuides"><h4>Revision Guides</h4></a>
        <nav class="nav nav-pills flex-column">
          <a class="nav-link ml-3 my-1" href="#inspector">An Inspector Calls</a>
          <a class="nav-link ml-3 my-1" href="#macbeth">Macbeth</a>
          <a class="nav-link ml-3 my-1" href="#othello">Othello</a>
        </nav>
      </nav>
    </nav>

    <div data-spy="scroll" data-target="#books-navbar" data-offset="0" class="col">
      <h3 id="11Plus">11+ workbooks for CEM style tests</h3>
    <ClozeCard id="cloze"></ClozeCard>
    <VocabWorkbookCard id="vocab"></VocabWorkbookCard>
    <ShortMathsTestsCard id="maths"></ShortMathsTestsCard>
    <ShuffledSentencesCard id="shuffled"></ShuffledSentencesCard>
    <SynAntCard id="synAnt"></SynAntCard>
    <SynAnt2Card id="synAnt2"></SynAnt2Card>
    <h3 id="revisionGuides">Revision Guides</h3>
      <InspectorCallsCard id="inspector"></InspectorCallsCard>
      <MacbethCard id="macbeth"></MacbethCard>
      <OthelloCard id="othello"></OthelloCard>
    </div>

  </div>
</template>

<script>// @ is an alias to /src
import ClozeCard from '@/components/BookCards/ClozeBookCard.vue'
import VocabWorkbookCard from '@/components/BookCards/VocabWorkbookCard.vue'
import ShortMathsTestsCard from '@/components/BookCards/ShortMathsTestsCard.vue'
import ShuffledSentencesCard from '@/components/BookCards/ShuffledSentencesCard.vue'
import SynAntCard from '@/components/BookCards/SynAntCard.vue'
import SynAnt2Card from '@/components/BookCards/SynAnt2Card.vue'
import InspectorCallsCard from '@/components/BookCards/InspectorCallsCard.vue'
import MacbethCard from '@/components/BookCards/MacbethCard.vue'
import OthelloCard from '@/components/BookCards/OthelloCard.vue'

export default {
  name: 'Books',
  components: {
    ClozeCard,
    VocabWorkbookCard,
    ShortMathsTestsCard,
    ShuffledSentencesCard,
    SynAntCard,
    SynAnt2Card,
    InspectorCallsCard,
    MacbethCard,
    OthelloCard
  }
}

</script>

<style scoped>
  a {
    color: #42b983;
  }

  .groupTitle{
    color: #232221
  }
</style>
