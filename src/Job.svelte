<script>
  export let client;
  export let when;
</script>

<style>
  .job {
    display: grid;
    grid-template-columns: var(--width-square-1) 1fr;
    column-gap: 1.5rem;
  }

  h3 {
    font-size: 1em;
    padding: 0 2rem 0 0;
    margin: 0;
    font-weight: 100;
    text-align: right;
  }

  ul {
    list-style: none;
  }
</style>

<div class="job">
  <header>
    <h3 class="when">{when}</h3>
    <h3>{client}</h3>
  </header>
  <ul>
    <slot />
  </ul>
</div>
