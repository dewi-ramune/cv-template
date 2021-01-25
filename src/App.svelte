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
    --clr-border: hsl(0, 0%, 0%);
    --width-border: 6px;
    --width-avatar: 48px;
    --width-square-1: 174px;
    --border: solid var(--width-border) var(--clr-border);
    --spacing: 0.8125rem;
    --spacing-1: calc(var(--spacing) / 4);
    --spacing-2: calc(var(--spacing) / 2);
    --spacing-5: calc(var(--spacing) * 2);
  }

  p {
    margin: 0;
  }

  @font-face {
    font-family: Slim Joe;
    src: url("./Slim Joe.otf") format("opentype");
  }

  * {
    font-size: 13px;
    color: var(--text-colour);
    box-sizing: border-box;
  }

  main {
    width: 794px;
    height: 1122px;
    display: grid;
    grid-template-columns: var(--width-square-1) 1fr var(--width-square-1);
    grid-template-rows: auto 1fr var(--width-square-1);
    background: url(../grid.svg);
    background-size: 100%;
    border: solid var(--width-border) var(--clr-border);
  }

  .content-section {
    display: flex;
    flex-direction: column;
    padding: 12px var(--width-border);
    position: relative;
  }

  .text-h3 {
    font-weight: 600;
    font-size: 13px;
    text-transform: uppercase;
  }

  .experience {
    grid-column: 1/-1;
    height: 100%;
    max-height: 100%;
    display: grid;
    grid-template-rows: auto repeat(4, auto 1fr) auto;
    border-bottom: solid var(--width-border) var(--clr-border);
  }
  .experience p {
    margin-bottom: 8px;
  }

  .education {
    display: flex;
    flex-direction: column;
  }

  .skills {
    display: grid;
    grid-template-columns: 1fr 1fr;
    grid-template-rows: 29px 18px auto 18px auto;
    column-gap: var(--spacing-5);
    border: solid var(--clr-border);
    border-width: 0 var(--width-border);
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
    margin-bottom: var(--spacing-2);
  }

  .section-header {
    font-family: "Slim Joe", Avenir, sans-serif;
    font-size: 22px;
    line-height: 1em;
    margin-bottom: 8px;
    text-transform: uppercase;
    font-weight: 600;
  }

  .emphasis {
    text-decoration: underline;
    text-decoration-color: hsla(52, 98%, 51%, 1);
    text-decoration-style: wavy;
  }

  .brackets::before {
    content: "(";
    font-weight: 600;
    color: hsla(52, 98%, 51%, 1);
  }
  .brackets::after {
    content: ")";
    font-weight: 600;
    color: hsla(52, 98%, 51%, 1);
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
      <Project role="DESIGN LEAD / UX DEVELOPER">
        <span slot="tools">
          <ToolTag tag="figma" />
          <ToolTag tag="react" />
          <ToolTag tag="css" />
        </span>
        <p>
          Design lead and UX developer to replace a legacy system with a bespoke
           CRM using <span class="emphasis">Elasticsearch / Cognito</span>. Built front-end in
          <span class="emphasis">React</span>
          with GraphQL integration and BDD using
          <span class="emphasis">Cypress</span>. I created a brand new design
          system and UI component library with an emphasis on user
          accessibility.
        </p>

        <p>
          I also led user research in order to formulate designs. First by
          contextual inquiry to gather requirements, map processes and identify
          bottlenecks. This was then translated into wireframes which I iterated
          over with users to ensure the solution was fit for purpose.
        </p>
      </Project>
    </Job>
    <b />

    <Job
            client="Intruder Systems"
            where="Tokyo / London"
            when="Aug 2020 - Current">
      <Project role="DESIGN LEAD / UX Prototyper">
        <span slot="tools">
          <ToolTag tag="figma" />
          <ToolTag tag="vue" />
        </span>
        <p>
          Used
          <span class="emphasis">Vue</span> and  <span class="emphasis">Tailwind</span>
         to deliver rapid prototyping of app restructure and rebrand. Worked closely with client's dev team to plan transition to new design.

        </p>

      </Project>
    </Job>
    <b />

    <Job client="Various Clients" where="London" when="Jun 2017 - Nov 2018">
      <Project role="Creative Technologist">
        <span slot="tools">
          <ToolTag tag="illustrator" />
          <ToolTag tag="photoshop" />
          <ToolTag tag="svg" />
          <ToolTag tag="vue" />
          <ToolTag tag="css" />
        </span>
        <p>
          Prototyped
          (<span class="emphasis">React / Vue</span>)
          several apps with a focus on point-of-sale systems (POS), including a
          self-service ordering / payment kiosk for KFC and a gas station kiosk
          for Orlen Stop Cafe to implement across their cafes nationwide.
        </p>
        <p>
          Produced original artwork and high-fidelity designs
          according to strict deadlines as well as creating branding guidance
          for the team, e.g. colour palettes, typefaces.
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
        <p>
          Designed
          and built
          responsive app UIs for an ambitious start-up to manage new client
          leads and distribute and manage event invitations and responses.
        </p>
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
          Responsible for ensuring compliance of commodities trading desk. Mentored and coached team of 6 analysts to deliver their best in a high-pressure environment.        </p>
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
      <div>
        <span class="text-h3">UNIVERSITY OF BATH</span>
        <p>BSc Hons Mathematics 2:1</p>
      </div>
    </div>
    <span />
  </div>

  <div class="content-section skills">
    <h2 class="section-header">Skills</h2>

    <span class="text-h3">DESIGN</span>
    <span class="text-h3">DEVELOPMENT</span>
    <div>
      <p>Figma</p>
      <p>Photoshop</p>
      <p>Illustrator</p>
      <p>Sketch</p>
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
      <p>Studying N5</p>
    </div>
  </div>
</main>
