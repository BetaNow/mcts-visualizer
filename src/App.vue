<template>
  <Header/>
  <main>
    <Setup/>
    <MCTSVisualizer/>
  </main>
</template>

<script>
import Setup from '@/Components/Setup.vue'
import Header from '@/Components/Header.vue'
import MCTSVisualizer from '@/Components/MCTSVisualizer.vue'

export default {
  components: { Header, Setup, MCTSVisualizer }
}
</script>

<style scoped lang="scss">
main {
  padding-top: 4rem;
  display: grid;
  grid-template-columns: 1fr 3fr;
  justify-items: center;
}
</style>
