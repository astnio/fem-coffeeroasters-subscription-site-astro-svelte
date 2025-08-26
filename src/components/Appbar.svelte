<script lang="ts">
  import Navigation from './Navigation.svelte';

  let { image } = $props();
</script>

<div class="appbar">
  <img src={image} alt="Coffeeroasters Logo" />
  <Navigation></Navigation>
</div>

<style lang="scss">
  .appbar {
    display: flex;
    align-items: center;
    justify-content: space-between;

    width: 100%;
  }
</style>
