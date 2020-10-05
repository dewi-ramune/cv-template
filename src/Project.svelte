<script>
  export let role;
</script>

<style>
  h3 {
    margin: 0 0 2px 0;
    padding: 0;
    font-size: 1em;
    font-weight: 600;
  }

  .project {
    display: flex;
    flex-direction: column;
  }
</style>

<li class="project">
  <h3>{role}</h3>
  <slot />
</li>
