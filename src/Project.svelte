<script>
  export let role;
</script>

<style>
  h3 {
    padding-bottom: 2px;
    font-size: 13px;
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
