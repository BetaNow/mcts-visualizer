<template>
  <header>
    <h1>MCTS Tic-tac-toe (Monte Carlo Tree Search) -&nbsp;</h1>
    <!-- Github button from: https://buttons.github.io/ -->
    <GithubButton href="https://github.com/BetaNow/mcts-visualizer" data-color-scheme="no-preference: light; light: light; dark: dark;" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star BetaNow/mcts-visualizer on GitHub">
      Star
    </GithubButton>
  </header>
</template>

<script>
import GithubButton from 'vue-github-button';

export default {
  components: { GithubButton }
}
</script>

<style scoped lang="scss">
header {
  display: flex;
  align-items: flex-end;
  justify-content: center;
  padding: 1rem;
  background-color: #f8f9fa;
  border-bottom: 1px solid #e9ecef;
}
</style>
