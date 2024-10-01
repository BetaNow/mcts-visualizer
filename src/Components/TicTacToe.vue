<template>
  <ul class="game">
    <li class="game__cell" v-for="cell in 9" :key="cell"></li>
  </ul>
</template>

<script>
export default {}
</script>

<style scoped lang="scss">
.game {
  width: 90%;
  aspect-ratio: 1 / 1;
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  border: 1px solid #222;
  border-right: none;
  border-bottom: none;

  &__cell {
    border: 1px solid #222;
    border-top: none;
    border-left: none;
  }
}
</style>
