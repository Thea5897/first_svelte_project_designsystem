<script>
  export let type = "default";
  export let mode;
</script>

<button class:inversed={mode === "inversed"} class={type}><slot /></button>

<style>
  button {
    border: black;
    padding: 6px;
    border-radius: 10px;
    padding-left: 10px;
    padding-right: 10px;
    margin: 0.5rem;
    color: white;
    background: var(--default-color);
    font-size: medium;
    cursor: pointer;
    transition: all 0.2s;
  }

  .primary {
    background-color: blue;
  }

  .primary:hover {
    color: var(--primary-color);
    background-color: var(--primary-font-color);
  }

  .primary.inversed {
    color: var(--primary-color);
    background-color: var(--primary-font-color);
  }

  .primary.inversed:hover {
    background-color: var(--primary-color);
    color: var(--primary-font-color);
  }

  .secondary {
    background-color: hotpink;
  }

  .secondary:hover {
    color: var(--secondary-color);
    background-color: var(--primary-font-color);
  }

  .secondary.inversed {
    color: var(--secondary-color);
    background-color: var(--primary-font-color);
  }

  .secondary.inversed:hover {
    background-color: var(--secondary-color);
    color: var(--primary-font-color);
  }

  .accent {
    background-color: var(--accent-color);
  }

  .accent.inversed {
    background-color: var(--primary-font-color);
    color: var(--accent-color);
  }

  .ghost {
    color: var(--ghost-font-color);
    background-color: var(--ghost-color);
  }

  .link {
    color: var(--link-color);
    background-color: var(--ghost-color);
  }
</style>
