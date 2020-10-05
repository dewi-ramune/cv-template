<style>
  header {
    grid-column: 1/-1;
    margin: 0;
    /* height: var(--width-square-1); */
    display: grid;
    grid-template-columns: var(--width-square-1) 1fr;
    grid-template-rows: 1fr auto;
    /* gap: var(--width-border); */
    align-items: center;
  }

  h1 {
    font-family: "Big John", Avenir, sans-serif;
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
    font-size: 22px;
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
    <!-- <span class="kana">ゴンザレス　デゥイ</span> -->
    <p>UX Designer / Developer</p>
  </div>

  <div class="content-section">
    <h2 class="section-header">profile</h2>
    <p>
      I am a visual & UX designer who has accidentally learned to love coding. I
      cover many aspects of design including animation, logos and layouts. I
      derive immense satisfaction from improving user experience and solving
      business problems through great design.
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
      <svg
        aria-hidden="true"
        focusable="false"
        width="26"
        height="26"
        class="svg-fill"
        role="img"
        xmlns="http://www.w3.org/2000/svg"
        viewBox="0 0 448 512"><path
          d="M424.7 299.8c2.9-14 4.7-28.9 4.7-43.8 0-113.5-91.9-205.3-205.3-205.3-14.9 0-29.7 1.7-43.8 4.7C161.3 40.7 137.7 32 112 32 50.2 32 0 82.2 0 144c0 25.7 8.7 49.3 23.3 68.2-2.9 14-4.7 28.9-4.7 43.8 0 113.5 91.9 205.3 205.3 205.3 14.9 0 29.7-1.7 43.8-4.7 19 14.6 42.6 23.3 68.2 23.3 61.8 0 112-50.2 112-112 .1-25.6-8.6-49.2-23.2-68.1zm-194.6 91.5c-65.6 0-120.5-29.2-120.5-65 0-16 9-30.6 29.5-30.6 31.2 0 34.1 44.9 88.1 44.9 25.7 0 42.3-11.4 42.3-26.3 0-18.7-16-21.6-42-28-62.5-15.4-117.8-22-117.8-87.2 0-59.2 58.6-81.1 109.1-81.1 55.1 0 110.8 21.9 110.8 55.4 0 16.9-11.4 31.8-30.3 31.8-28.3 0-29.2-33.5-75-33.5-25.7 0-42 7-42 22.5 0 19.8 20.8 21.8 69.1 33 41.4 9.3 90.7 26.8 90.7 77.6 0 59.1-57.1 86.5-112 86.5z" /></svg>
    </div>
    <p>dewiwaugh</p>
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
