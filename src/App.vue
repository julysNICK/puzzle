<template>
  <div>

    <PuzzlesComponent @puzzle-changed="selectedPuzzleId = $event" />
    <RecordsComponent />
    <SliderPuzzleComponent :puzzle-id="selectedPuzzleId" />

  </div>
</template>

<script>
import SliderPuzzleComponent from './components/SliderPuzzle.vue'
import PuzzlesComponent from './components/Puzzles.vue'
import RecordsComponent from './components/Records.vue'

export default {
  name: 'App',
  components: {
    SliderPuzzleComponent,
    PuzzlesComponent,
    RecordsComponent
  },

  data() {
    return {
      selectedPuzzleId: "cut-pink"
    }
  }
}
</script>

<style></style>
