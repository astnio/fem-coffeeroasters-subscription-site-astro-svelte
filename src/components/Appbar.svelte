<script lang="ts">
  import Navigation from './Navigation.svelte';

  let { image } = $props();
</script>

<div class="appbar">
  <div class="appbar-content max-width">
    <img src={image} alt="Coffeeroasters Logo" />
    <Navigation></Navigation>
  </div>
</div>

<style lang="scss">
  @use '/src/styles/variables' as *;

  .appbar {
    position: fixed;
    top: 0;
    left: 0;

    z-index: 10;

    display: flex;
    align-items: center;
    justify-content: center;

    width: 100%;

    margin-inline: auto;
    padding-block: 1rem;

    background-color: white;
  }

  .appbar-content {
    display: flex;
    align-items: center;
    justify-content: space-between;
  }
</style>
