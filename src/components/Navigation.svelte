<nav>
  <ol>
    <li><a href="/">Home</a></li>
    <li><a href="/about">About us</a></li>
    <li><a href="plan">Create your plan</a></li>
  </ol>
</nav>

<style lang="scss">
  @use '/src/styles/variables' as *;

  nav {
    display: flex;
    align-items: center;
    justify-content: space-between;
  }

  ol {
    display: flex;
    gap: 1rem;

    list-style-type: none;

    margin: 0;
    padding: 0;
  }

  a {
    text-decoration: none;
    font-weight: 700;
    text-transform: uppercase;
    color: $clr-grey;
  }
</style>
