<script></script>

<button class="button btn-primary">
  <slot></slot>
</button>

<style lang="scss">
  @use '/src/styles/variables' as *;

  .button {
    display: flex;
    align-items: center;
    justify-content: center;

    border: none;
    border-radius: 6pt;

    padding-block: 1rem;
    padding-inline: 1rem;

    width: 100%;
    max-width: 12rem;

    font-family: 'Fraunces', serif;
    font-weight: 700;
    font-size: 1rem;
  }

  .button.btn-primary {
    background-color: $clr-dark-cyan;
    color: $clr-light-cream;
  }
</style>
