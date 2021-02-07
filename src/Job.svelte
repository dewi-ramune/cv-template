<script>
  export let client;
  export let when;
  export let where;
</script>

<style>
  .job {
    display: grid;
    grid-template-columns: var(--width-square-1) 1fr;
  }

  h3 {
    font-size: 13px;
    padding: 0 3rem 0 0;
    text-align: right;
  }

  .who {
    padding-bottom: 2px;
    font-size: 12px;
    font-weight: 600;
    text-transform: uppercase;  }
  .where {
    display: none;
  }

  ul {
    list-style: none;
  }
</style>

<div class="job">
  <header>
    <h3 class="who">{client}</h3>
    <h3 class="when">{when}</h3>
    <h3 class="where">{where}</h3>
  </header>
  <ul>
    <slot />
  </ul>
</div>
