<script>
  export let type = "default";
  export let mode = "default";
</script>

<button class:inversed={mode === "inversed"} class={type}><slot /></button>

<style>
  button {
    color: var(--primary-font-color);
    background-color: slategrey;
    transition: 0.2s ease;
    padding: 1rem 2rem;
    text-transform: uppercase;
    border-radius: 0.5rem;
    border: none;
    font-weight: 800;
    cursor: pointer;
    display: inline-block;
  }

  .primary {
    background: var(--primary-color);
  }

  button:hover {
    filter: brightness(0.7);
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

  .link {
    background-color: transparent;
    color: var(--link-font-color);
  }

  .primary.inversed {
    background-color: var(--primary-font-color);
    color: var(--link-font-color);
  }
</style>
