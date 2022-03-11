<script>
  export let type = "default";
  export let mode = "default";
</script>

<div class:inversed={mode === "inversed"} class={type}><slot /></div>

<style>
  div {
    color: var(--primary-font-color);
    background-color: slategrey;
    transition: 250ms ease-in-out;
    padding: 0.2rem 0.4rem;
    text-transform: lowercase;
    border-radius: 1rem;
    border: none;

    display: inline-block;
  }

  .primary {
    background: var(--primary-color);
  }

  .secondary {
    background-color: var(--secondary-color);
  }

  .accent {
    background-color: var(--accent-color);
  }

  .ghost {
    background-color: transparent;
    color: var(--secondary-font-color);
  }

  .border {
    background-color: transparent;
    color: var(--secondary-font-color);
    border: 2px solid var(--secondary-font-color);
  }

  .link {
    background-color: transparent;
    color: var(--link-font-color);
  }

  .primary.inversed {
    background-color: var(--primary-font-color);
    color: var(--link-font-color);
  }
</style>
