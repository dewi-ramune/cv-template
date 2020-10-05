<script>
  import Header from "./Header.svelte";
  import Job from "./Job.svelte";
  import Project from "./Project.svelte";
  import ToolTag from "./ToolTag.svelte";
</script>

<style>
  :root {
    --text-colour: hsl(220, 100%, 0%);
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
    grid-template-columns: var(--width-square-1) 1fr var(--width-square-1);
    grid-template-rows: var(--width-square-1) 751px var(--width-square-1);
    gap: var(--width-border);
    padding: var(--width-border);
    background: url(../grid.svg);
    background-size: 100%;
  }

  .content-section {
    display: flex;
    flex-direction: column;
    padding: var(--width-border);
    position: relative;
  }

  .text-h3 {
    font-weight: 600;
    font-size: 1rem;
    text-transform: uppercase;
  }

  .experience {
    grid-column: 1/-1;
    height: 100%;
    max-height: 100%;
    display: grid;
    grid-template-rows: auto repeat(4, auto 1fr) auto 1rem;
  }

  .education {
    display: flex;
    flex-direction: column;
  }

  .skills {
    display: grid;
    grid-template-columns: 1fr 1fr;
    grid-template-rows: 33px 1.5rem auto 1.5rem auto;
    column-gap: var(--spacing-5);
  }
  .skills > .section-header {
    grid-column: 1/-1;
  }

  .skills p {
    display: inline-block;
  }
  .skills p:not(:last-child)::after {
    content: "\00a0\25cf\00a0";
  }

  .skill-block {
    margin: var(--spacing-2) 0;
    display: grid;
  }

  .skill-block.first {
    margin-top: 0;
  }

  .section-header {
    font-size: 21px;
    line-height: 1em;
    margin: 0 0 var(--spacing-2) 0;
    text-transform: uppercase;
    font-weight: 600;
  }

  li {
    list-style-position: inside;
  }
</style>

<main>
  <Header />

  <div class="content-section experience">
    <h2 class="section-header">Experience</h2>
    <Job
      client="A2B Assessments"
      where="Tokyo / London"
      when="Nov 2018 - Current">
      <Project role="DESIGN LEAD / DEVELOPER">
        <span slot="tools">
          <ToolTag tag="figma" />
          <ToolTag tag="react" />
          <ToolTag tag="css" />
        </span>
        <p>
          Design lead and main front-end developer to replace a legacy system
          with a bespoke cloud-based CRM. Front-end built in React with GraphQL
          integration and BDD integration testing in Cypress. I created a brand
          new design system and UI component library with an emphasis on user
          accessibility.
        </p>

        <p>
          I also lead user research in order to understand and streamline
          business processes. First I mapped their processes, and then regularly
          met users to iterate through designs and wireframes to ensure the
          solution was fit for purpose.
        </p>

        <p>
          Currently I am prototyping a new reporting feature whilst adding to
          their design system.
        </p>
      </Project>
    </Job>
    <b />

    <Job client="Various Clients" where="London" when="Jun 2017 - Nov 2018">
      <Project role="UX PROTOTYPER">
        <span slot="tools">
          <ToolTag tag="illustrator" />
          <ToolTag tag="photoshop" />
          <ToolTag tag="svg" />
          <ToolTag tag="vue" />
          <ToolTag tag="css" />
        </span>
        <p>
          Prototyped several apps in React/Vue with a focus on point-of-sale
          systems (POS), e.g.
          <li>
            gas station kiosk for Orlen Stop Cafe to implement across their
            cafes nationwide.
          </li>
          <li>self-service ordering/payment kiosk for KFC</li>
        </p>
        <p>
          Deadlines were very strict which meant rapid prototyping in React/Vue
          as well as creating original artwork and branding guidance to the
          team, e.g. colour palettes, typefaces.
        </p>
      </Project>
    </Job>
    <b />
    <Job client="CREAT3D" where="Reading" when="Jan 2017 - Feb 2018">
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
    <b />

    <Job client="EDF Energy" where="London" when="Jan 2012 - Nov 2016">
      <Project role="RISK OPERATIONS MANAGER">
        <span slot="tools">
          <ToolTag tag="javascript" />
          <ToolTag tag="html" />
          <ToolTag tag="css" />
        </span>
        <p>
          Managed a team of 6 analysts to provide accurate and timely MI
          reporting. Transformed verbose risk regulation guidelines into a
          user-friendly web portal.
        </p>
      </Project>
      <Project role="SENIOR BUSINESS ANALYST">
        <p>
          Responsible for stakeholder engagement across 15 different teams for
          organization-wide trading system replacement project.
        </p>
      </Project>
      <Project role="SENIOR ANALYST">
        <p>
          Performed data analysis and built various models and tools in VBA, MS
          Excel, MS Access, SQL, MatLab, e.g. forecasting energy prices, value
          at risk, PCA.
        </p>
      </Project>
    </Job>
    <b />

    <Job client="Marubeni" where="London" when="Oct 2008 - Dec 2011">
      <Project role="ANALYST">
        <p>
          Worked across teams for their UK-based energy trading subsidiary.
          Selected from over 29,000 employees worldwide to attend annual
          training workshop at Tokyo HQ.
        </p>
      </Project>
    </Job>
  </div>

  <div class="education">
    <div class="content-section">
      <h2 class="section-header">Education</h2>
      <div class="skill-block first">
        <span class="text-h3">UNIVERSITY OF BATH, UK</span>
        <p>BSc (Hons) Mathematics 2:1</p>
      </div>
    </div>
    <span />
  </div>

  <div class="content-section skills">
    <h2 class="section-header">Skills</h2>

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

  <div class="content-section">
    <h2 class="section-header">Languages</h2>

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
</main>
