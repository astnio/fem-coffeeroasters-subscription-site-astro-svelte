<script lang="ts">
  import Navigation from './Navigation.svelte';

  let { image } = $props();
</script>

<header class="appbar max-width">
  <div class="appbar-content max-width">
    <img src={image} alt="Coffeeroasters Logo" />
    <Navigation></Navigation>
  </div>
</header>

<style lang="scss">
  @use '/src/styles/variables' as *;

  .appbar {
    position: sticky;
    top: 0rem;

    z-index: 10;

    display: flex;
    align-items: center;
    justify-content: center;

    width: 100%;

    margin-inline: auto;
    padding-block: 2rem;

    background-color: white;
  }

  .appbar-content {
    display: flex;
    align-items: center;
    justify-content: space-between;
  }
</style>
