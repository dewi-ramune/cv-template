<script>
</script>

<style>
  header {
    grid-column: 1/-1;
    margin: 0;
    height: var(--width-square-1);
    display: grid;
    grid-template-columns: var(--width-square-1) 1fr;
    grid-template-rows: 1fr auto;
    align-items: center;
    /* border-bottom: var(--border); */
  }

  h1 {
    font-size: 3em;
    line-height: 1.125em;
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
    box-sizing: border-box;
    position: relative;
  }

  .profile {
    padding: var(--spacing);
  }
  .profile p:not(:last-child) {
    margin-bottom: var(--spacing);
  }

  img {
    /* position: absolute; */
    display: block;
    top: 0;
    right: 0;
    width: var(--width-avatar);
    height: var(--width-avatar);
    object-fit: scale-down;
    border-radius: 0 0 0 50%;
  }

  .name {
    padding: var(--spacing);
    grid-row: 1/-1;
    position: relative;
    display: flex;
    flex-direction: column;
    height: 100%;
  }

  .contact {
    display: grid;
    grid-template-columns: repeat(3, 40px max-content 1fr);
    gap: var(--width-border);
    padding: 0 var(--width-border);
  }
  .contact > p {
    padding: var(--spacing) var(--width-border);
  }

  .feather {
    display: block;
    stroke: black;
    stroke-width: 2;
    stroke-linecap: round;
    stroke-linejoin: round;
  }
</style>

<header>
  <div class="name">
    <!-- <img alt="avatar" src="dewi.svg" /> -->

    <h1>
      Dewi
      <br />
      Gonzalez
    </h1>
    <!-- <h2>ゴンザレス　デゥイ</h2> -->
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

  <div class="contact">
    <svg
      xmlns="http://www.w3.org/2000/svg"
      width="24"
      height="24"
      viewBox="0 0 24 24"
      class="feather">
      <path
        d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z" />
      <polyline points="22,6 12,13 2,6" />
    </svg>
    <p>dewi@ramune.io</p>
    <b />
    <svg
      xmlns="http://www.w3.org/2000/svg"
      width="24"
      height="24"
      viewBox="0 0 24 24"
      class="feather">
      <path
        d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z" />
      <polyline points="22,6 12,13 2,6" />
    </svg>
    <p>dewiwaugh</p>
    <b />
    <b />
    <p>https://dewi.ramune.io/</p>
    <b />
  </div>
</header>
