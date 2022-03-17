<script>
  import Badge from "./Badge.svelte";
  import Button from "./Button.svelte";
</script>

<div class="bb_container">
  <div id="button"><Button type="primary">Inbox</Button></div>
  <div id="badge"><Badge type="secondary">99+</Badge></div>
</div>

<style>
  #badge {
    position: absolute;
    left: 50vw;
    top: 154vh;
  }
</style>
