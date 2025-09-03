<script>
  import logoImageDark from '../assets/shared/desktop/logo.svg';
  import logoImageLight from '../assets/shared/desktop/logo_light.svg';
  let { darkMode } = $props();
</script>

<a href="/">
  <img
    src={darkMode ? logoImageLight.src : logoImageDark.src}
    alt="Coffeeroasters Logo"
  />
</a>
