<script>
  export let className = "";
  export let tag;
</script>

<style>
  :root {
    --react: 189, 80%, 50%;
    --sketch: 37, 100%, 50%;
    --css: 45, 99%, 50%;
    --illustrator: 15, 98%, 58%;
    --vue: 169, 100%, 37%;
    --svg: 234, 45%, 48%;
    --javascript: 245, 81%, 69%;
    --figma: 352, 79%, 56%;
    --photoshop: 209, 100%, 65%;
    --html: 185, 100%, 32%;
  }

  label {
    border-radius: 4px;
    padding: 1px 6px;
  }

  .tag {
    color: white;
    font-weight: 500;
  }

  .figma {
    background-color: hsla(var(--figma), 1);
  }

  .html {
    background-color: hsla(var(--html), 1);
  }

  .react {
    background-color: hsla(var(--react), 1);
  }

  .css {
    background-color: hsla(var(--css));
  }

  .illustrator {
    background-color: hsla(var(--illustrator), 1);
  }

  .photoshop {
    background-color: hsla(var(--photoshop), 1);
  }

  .sketch {
    background-color: hsla(var(--sketch), 1);
  }

  .vue {
    background-color: hsla(var(--vue), 1);
  }

  .svg {
    background-color: hsla(var(--svg));
  }

  .javascript {
    background-color: hsla(var(--javascript), 1);
  }
</style>

<label class={`tag ${tag} ${className}`}>{tag}</label>
