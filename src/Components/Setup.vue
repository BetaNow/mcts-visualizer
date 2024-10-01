<template>
  <div class="game">
    <TicTacToe  />

    <div class="game-start">
      <h3>Who will start the game?</h3>
      <button>Human</button>
      <button>Machine</button>
    </div>

    <div class="game-turn">
      <h3 v-if="isHumanTurn">It's your turn!</h3>
      <h3 v-else>It's the machine's turn!</h3>
    </div>

    <div class="game-controls">
      <h3>Machine controls:</h3>
      <button>Make random move</button>
      <button>Make MCTS move</button>
      <label for="iteration">Run MCTS for:</label>
      <input v-model="iteration" type="range" name="iteration" id="iteration" min="100" max="2000">
      <p>{{ iteration }} Iteration</p>
    </div>

    <div class="game-winner">
      <h3 v-if="isHumanTurn">You win!</h3>
      <h3 v-else>The machine wins!</h3>
      <button>Restart the game</button>
    </div>
  </div>
</template>

<script>
import TicTacToe from '@/Components/TicTacToe.vue'

export default {
  components: { TicTacToe },
  data () {
    return {
      isHumanTurn: false,
      iteration: 1000,
    }
  }
}
</script>

<style scoped lang="scss">
.game {
  width: 90%;
}
</style>
