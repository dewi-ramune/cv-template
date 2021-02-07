<script>
  export let role;
</script>

<style>
  h3 {
    padding-bottom: 2px;
    font-size: 12px;
    font-weight: 600;
    text-transform: uppercase;
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
