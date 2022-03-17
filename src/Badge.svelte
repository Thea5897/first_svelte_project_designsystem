<script>
  export let type = "default";
</script>

<span class={type}>
  <slot />
</span>

<style>
  span {
    background-color: white;
    border-radius: 10px;
    padding: 6px;
    margin: 2px;
    background: var(--default-color);
    color: var(--primary-font-color);

    width: 10vh;
  }

  .primary {
    color: var(--primary-font-color);
    background-color: var(--primary-color);
  }

  .secondary {
    background-color: hotpink;
    color: var(--primary-font-color);
  }
  .accent {
    background-color: var(--accent-color);
  }

  .ghost {
    color: var(--ghost-font-color);
    background-color: var(--ghost-color);
    border-style: ridge;
  }

  .link {
    color: var(--link-color);
    background-color: var(--ghost-color);
  }
</style>
