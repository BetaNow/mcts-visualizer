<template>
  <div class="visualizer">
    <div class="visualizer-controls">
      <div class="actions">
        <h3>Current action:</h3>
        <p>(-/-)</p>
        <p>---</p>
        <button>next action ></button>
      </div>

      <div class="iterations">
        <h3>Current iteration:</h3>
        <p>(-/-)</p>
        <br>
        <button>next iteration >></button>
      </div>

      <div class="step">
        <button>Visualize last step >>></button>
        <button>Make Play</button>
      </div>
    </div>

    <div class="visualizer-graph"></div>
  </div>
</template>

<script>
export default {}
</script>

<style scoped lang="scss">
.visualizer {
  border: 1px solid #222;
  width: 90%;
  height: 80vh;

  &-controls {
    display: flex;
    gap: 1rem;
  }

  &-graph {
    border-top: 1px solid #222;
    width: 100%;
    height: 100%;
  }
}
</style>
