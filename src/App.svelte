<script>
  import Header from "./Header.svelte";
  import Job from "./Job.svelte";
  import Project from "./Project.svelte";
  import ToolTag from "./ToolTag.svelte";
  import ProjectContent from "./ProjectContent.svelte";
</script>

<style>
  :root {
    --text-colour: hsl(220, 100%, 20%);
    --primary: hsl(0, 0%, 90%);
    --bgrd: hsl(350, 100%, 97%);
    --clr-border: hsl(0, 0%, 100%);
    --width-border: 6px;
    --width-avatar: 48px;
    --width-square-1: 174px;
    --border: solid var(--width-border) var(--clr-border);
    --spacing: 1em;
    --spacing-1: calc(var(--spacing) / 4);
    --spacing-2: calc(var(--spacing) / 2);
    --spacing-5: calc(var(--spacing) * 2);
  }

  p {
    margin: 0;
  }

  * {
    color: var(--text-colour);
    box-sizing: border-box;
  }

  main {
    display: grid;
    grid-template-columns: var(--width-square-1) var(--width-square-1) 1fr;
    grid-template-rows: var(--width-square-1) 751px var(--width-square-1);
    gap: var(--width-border);
    background-color: var(--bgrd);
    padding: var(--width-border);
    /* background: url(../grid.svg); */
    background-size: 100%;
  }

  .content-section {
    display: flex;
    flex-direction: column;
    padding: var(--width-border);
    position: relative;
  }

  .section-header {
    font-size: 1.75em;
    margin: 0 0 var(--spacing-2) 0;
    text-transform: uppercase;
  }

  .skill-block {
    margin: var(--spacing-2) 0;
    display: grid;
  }

  .skill-block.first {
    margin-top: 0;
  }

  .skills p {
    display: inline-block;
  }
  .skills p:not(:last-child)::after {
    content: "\00a0\25cf\00a0";
    /* content: "\00a0\2b24\00a0";
    font-size: 0.75rem; */
    /* color: var(--clr-border); */
  }

  .text-h3 {
    font-weight: 600;
    font-size: 1rem;
    text-transform: uppercase;
  }

  .experience {
    grid-column: 2/-1;
    /* border-bottom: var(--border); */
    height: 100%;
    max-height: 100%;
  }

  .education {
    /* border-right: var(--border); */
    display: flex;
    flex-direction: column;
  }

  .skills {
    /* border-right: var(--border); */
    display: grid;
    grid-template-columns: 1fr 1fr;
    grid-template-rows: 33px 1.5rem auto 1.5rem auto;
    column-gap: var(--spacing-5);
    /* background: repeating-linear-gradient(
      0deg,
      transparent,
      transparent var(--width-border),
      var(--clr-border) var(--width-border),
      var(--clr-border) calc(2 * var(--width-border))
    ); */
  }
  .skills > header {
    grid-column: 1/-1;
  }

  .stripes {
    height: 100%;
    background: repeating-linear-gradient(
      90deg,
      transparent,
      transparent var(--width-border),
      var(--clr-border) var(--width-border),
      var(--clr-border) calc(2 * var(--width-border))
    );
    border-top: var(--border);
  }
</style>

<main>
  <Header />

  <div class="content-section">
    <header class="section-header">Experience</header>
  </div>
  <div class="content-section experience">
    <Job
      client="A2B Assessments"
      where="Tokyo / London"
      when="Nov-18 – Current">
      <Project role="DESIGN LEAD / DEVELOPER">
        <span slot="tools">
          <ToolTag tag="figma" />
          <ToolTag tag="react" />
          <ToolTag tag="css" />
        </span>
        <li>
          Design lead and main front-end developer to replace a
          spreadsheet-based legacy system with a bespoke cloud-based CRM.
        </li>
        <li>
          Built and maintained a brand new design system and UI component
          library with an emphasis on user accessibility.
        </li>
        <li>Created wireframes / prototypes.</li>
        <li>
          Engaged users in weekly meetings to iterate through designs and ensure
          prototypes were fit for purpose.
        </li>
        <li>
          Front-end development with GraphQL integration and BDD integration
          testing in Cypress.
        </li>
        <li>Ran workshops and shadowed users to gather requirements.</li>
        <li>Produced and maintained user journeys and process maps.</li>
      </Project>
    </Job>

    <Job client="Various Clients" where="London" when="Jun-17 – Nov-18">
      <Project role="CREATIVE TECHNOLOGIST">
        <span slot="tools">
          <ToolTag tag="illustrator" />
          <ToolTag tag="photoshop" />
          <ToolTag tag="svg" />
          <ToolTag tag="vue" />
          <ToolTag tag="css" />
        </span>
        <li>
          Designed a gas station kiosk prototype for Orlen Stop Cafe to
          implement across their cafes nationwide.
        </li>
        <li>
          Designed a self-service kiosk protoype for KFC to be demoed at a
          tradeshow.
        </li>
        <li>
          Logo design and branding guidance, e.g. colour palettes, typefaces.
        </li>
        <li>
          Collaborated with project team to prepare proposals, wireframes and
          original artwork for client bids.
        </li>
      </Project>
    </Job>

    <Job client="CREAT3D" where="Reading" when="Jan-17 – Feb-18">
      <Project role="DESIGNER / FRONT-END DEVELOPER">
        <span slot="tools">
          <ToolTag tag="sketch" />
          <ToolTag tag="vue" />
          <ToolTag tag="css" />
        </span>
        <li>
          Designed and built UI for a mobile app to distribute and manage
          invitations and responses to company events.
        </li>
        <li>
          Designed and built UI for a company branded mobile app to collect
          customer details at trade events.
        </li>
      </Project>
    </Job>

    <Job client="EDF Energy" where="London" when="Jan-12 – Nov-16">
      <Project role="RISK OPERATIONS MANAGER">
        <span slot="tools">
          <ToolTag tag="javascript" />
          <ToolTag tag="html" />
          <ToolTag tag="css" />
        </span>
        <li>
          Managed a team of 6 analysts to provide accurate and timely MI
          reporting.
        </li>
        <li>
          Collaborated with project team to prepare proposals, wireframes and
          original artwork for client bids.
        </li>
      </Project>
      <Project role="SENIOR BUSINESS ANALYST">
        <li>
          Responsible for stakeholder engagement across 15 different teams for
          organization-wide trading system replacement project.
        </li>
      </Project>
      <Project role="SENIOR ANALYST">
        <li>
          Performed data analysis and built various models and tools in VBA, MS
          Excel, MS Access, SQL, MatLab, e.g. forecasting energy prices, value
          at risk, PCA.
        </li>
      </Project>
    </Job>

    <Job client="Marubeni" where="London" when="Oct-08 – Dec-11">
      <Project role="ANALYST">
        <li>
          Selected from over 29,000 employees worldwide to attend annual
          training workshop at Tokyo HQ.
        </li>
      </Project>
    </Job>
  </div>

  <div class="education">
    <div class="content-section">
      <header class="section-header">Education</header>
      <div class="skill-block first">
        <span class="text-h3">UNIVERSITY OF BATH, UK</span>
        <p>BSc (Hons) Mathematics 2:1</p>
      </div>
    </div>
    <span class="stripes" />
  </div>

  <div class="content-section">
    <header class="section-header">Languages</header>

    <div class="skill-block first">
      <span class="text-h3">ENGLISH</span>
      <p>Native</p>
    </div>

    <div class="skill-block">
      <span class="text-h3">INDONESIAN</span>
      <p>Fluent</p>
    </div>

    <div class="skill-block">
      <span class="text-h3">JAPANESE</span>
      <p>Studying N4</p>
    </div>
  </div>

  <div class="content-section skills">
    <header class="section-header">Skills</header>

    <span class="text-h3">DESIGN</span>
    <span class="text-h3">DEVELOPMENT</span>
    <div>
      <p>Photoshop</p>
      <p>Illustrator</p>
      <p>XD</p>
      <p>Sketch</p>
      <p>Figma</p>
      <p>Storybook</p>
      <p>pen & paper</p>
    </div>
    <div>
      <p>HTML</p>
      <p>CSS</p>
      <p>SVG</p>
      <p>JavaScript</p>
      <p>React</p>
      <p>Vue</p>
      <p>Svelte</p>
      <p>Cypress</p>
      <p>Cucumber</p>
    </div>

    <span class="text-h3">ASSET MANAGEMENT</span>
    <span class="text-h3">PLANNING</span>
    <div>
      <p>Git</p>
      <p>Creative Cloud</p>
    </div>
    <div>
      <p>Trello</p>
      <p>Asana</p>
      <p>Agile</p>
    </div>
  </div>
</main>
