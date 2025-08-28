<script lang="ts">
  import Navigation from './Navigation.svelte';

  let { image } = $props();
</script>

<header class="appbar">
  <div class="appbar-content max-width">
    <a href="/">
      <img src={image} alt="Coffeeroasters Logo" />
    </a>
    <Navigation></Navigation>
  </div>
</header>

<style lang="scss">
  @use '/src/styles/variables' as *;

  .appbar {
    position: sticky;
    top: 0rem;

    margin-top: 1.5rem;

    z-index: 10;

    display: flex;
    align-items: center;
    justify-content: center;

    width: 100%;

    margin-inline: auto;
    padding-block: 1rem;

    backdrop-filter: blur(10px);
  }

  .appbar::after {
    content: '';
    position: absolute;
    left: 0;
    top: 0;

    width: 100%;
    height: 100%;

    background-color: white;
    opacity: 0.8;

    z-index: -1;
  }

  .appbar-content {
    display: flex;
    align-items: center;
    justify-content: space-between;

    padding-inline: 4rem;
  }
</style>
