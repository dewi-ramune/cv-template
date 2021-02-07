<style>
  header {
    grid-column: 1/-1;
    margin: 0;
    display: grid;
    grid-template-columns: var(--width-square-1) 1fr;
    grid-template-rows: 1fr auto;
    align-items: center;
  }

  h1 {
    font-size: 27px;
    line-height: 1.125em;
    padding: 0;
    margin: 0;
    font-weight: 500;
  }

  p {
    margin: 0;
  }

  header > div {
    box-sizing: border-box;
  }

  .name {
    padding: 12px var(--width-border);
    grid-row: 1/-1;
    position: relative;
    display: flex;
    flex-direction: column;
    height: 100%;
    border-bottom: solid var(--width-border) var(--clr-border);
  }
  .name p {
    padding-top: 0.5rem;
  }

  .contact {
    display: grid;
    grid-template-columns: repeat(3, 40px max-content 1fr);
    gap: var(--width-border);
    border: solid var(--clr-border);
    border-width: var(--width-border) 0;
  }
  .contact > p {
    padding: 11px;
  }

  .feather {
    display: block;
    stroke: white;
    fill: none;
    stroke-width: 3;
    stroke-linecap: round;
    stroke-linejoin: round;
    margin: auto;
    opacity: 0.7;
  }

  .svg-fill {
    display: block;
    fill: white;
    margin: auto;
    opacity: 0.8;
  }

  .icon {
    width: 100%;
    display: flex;
    border: solid var(--clr-border);
    border-width: 0 var(--width-border);
  }

  .icon:nth-of-type(1) {
    background-color: hsla(241, 100%, 64%, 1);
  }
  .icon:nth-of-type(2) {
    background-color: hsla(1, 97%, 59%, 1);
  }
  .icon:nth-of-type(3) {
    background-color: hsla(52, 98%, 51%, 1);
  }

  .content-section {
    display: flex;
    flex-direction: column;
    padding: 12px var(--width-border);
    position: relative;
    border-left: solid var(--width-border) var(--clr-border);
  }

  .section-header {
    font-family: "Slim Joe", Avenir, sans-serif;
    font-size: 18px;
    line-height: 1em;
    margin-bottom: 8px;
    text-transform: uppercase;
    font-weight: 600;
  }
</style>

<header>
  <div class="name">
    <!-- <img alt="avatar" src="dewi.svg" /> -->
    <h1>Dewi <br /> Gonzalez</h1>
<!--     <span class="kana">ゴンザレス　デゥイ</span>-->
    <p>UX Designer / Developer</p>
  </div>

  <div class="content-section">
    <h2 class="section-header">profile</h2>
    <p>
      I am a UX designer who accidentally learned to love coding. As the co-founder of a software consultancy, I am adept at presenting to stakeholders and balancing multiple projects. Able to take ideas from conceptualization all the way through to wireframing, prototyping and production.
    </p>
  </div>

  <div class="contact">
    <div class="icon">
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
    </div>
    <p>dewi@ramune.io</p>
    <b />

    <div class="icon">


      <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-phone"><path d="M22 16.92v3a2 2 0 0 1-2.18 2 19.79 19.79 0 0 1-8.63-3.07 19.5 19.5 0 0 1-6-6 19.79 19.79 0 0 1-3.07-8.67A2 2 0 0 1 4.11 2h3a2 2 0 0 1 2 1.72 12.84 12.84 0 0 0 .7 2.81 2 2 0 0 1-.45 2.11L8.09 9.91a16 16 0 0 0 6 6l1.27-1.27a2 2 0 0 1 2.11-.45 12.84 12.84 0 0 0 2.81.7A2 2 0 0 1 22 16.92z"></path></svg>    </div>
    <p>080 5961 5903</p>
    <b />

    <div class="icon">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        width="24"
        height="24"
        viewBox="0 0 24 24"
        class="feather"><rect
          x="2"
          y="3"
          width="20"
          height="14"
          rx="2"
          ry="2" />
        <line x1="8" y1="21" x2="16" y2="21" />
        <line x1="12" y1="17" x2="12" y2="21" /></svg>
    </div>
    <p>https://dewi.ramune.io/</p>
    <b />
  </div>
</header>
