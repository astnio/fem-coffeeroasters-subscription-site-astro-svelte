<script>
  let { children, link } = $props();
</script>

<a href={link} class="button btn-primary">
  {@render children?.()}
</a>

<style lang="scss">
  @use '/src/styles/variables' as *;

  a.button {
    display: flex;
    align-items: center;
    justify-content: center;

    border: none;
    border-radius: 6pt;

    padding-block: 1rem;
    padding-inline: 0.5rem;

    margin: 0;

    width: 100%;
    max-width: 12rem;

    font-family: 'Fraunces', serif;
    font-weight: 700;
    font-size: 1rem;
    text-decoration: none;

    cursor: pointer;

    transition-property: background-color;
    transition-duration: 0.1s;
    transition-timing-function: ease-out;
  }

  a.button.btn-primary {
    background-color: $clr-primary;
    color: $clr-light-cream;
  }

  a.button.btn-primary:active,
  a.button.btn-primary:hover {
    background-color: $clr-primary-active;
  }
</style>
