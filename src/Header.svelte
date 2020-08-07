<script>

</script>

<style>
  header {
    grid-column: 1/-1;
    margin: 0;
    display: grid;
    grid-template-columns: max-content 1fr;
    align-items: center;
    border-bottom: var(--border);
  }

  h1 {
    font-size: 2em;
    padding: 0;
    margin: 0;
  }
  h2 {
    font-weight: normal;
    font-size: 1em;
  }

  p {
    margin: 0;
  }

  header > div {
    padding: var(--spacing);
  }

  .profile {
    border-left: var(--border);
  }
  .profile p:not(:last-child) {
    margin-bottom: var(--spacing);
  }
</style>

<header>
  <div class="name">
    <h1>Dewi Gonzalez</h1>
    <h2>ゴンザレス　デゥイ</h2>
    <p>UX Designer / Developer</p>
  </div>

  <div class="content-section profile">
    <p>
      After many years of crunching numbers I decided to pivot and pursue a
      career in design. Since then I have produced artwork and UI prototypes for
      fun clients like KFC. I derive immense satisfaction from improving user
      experience and solving business problems through great design.
    </p>
    <p>I also love food, films and creating kawaii animal SVGs.</p>
  </div>
</header>
