<script>
  import Badge from "./Badge.svelte";
  export let description;
  import Button from "./Button.svelte";
</script>

<div class="card">
  <div class="img" />
  <img src="./horizon.jpg" alt="Horizon" class="billede" />
  <div>
    <div class="wrap">
      <h3><slot />!</h3>
      <Badge type="secondary">NEW</Badge>
    </div>

    <p>{description}</p>
    <Badge type="ghost">Fashion</Badge><Badge type="ghost">Products</Badge>
  </div>
  <br />
  <Button type="primary">Køb nu!</Button>
</div>

<style>
  .billede {
    height: 22vh;
    margin-top: 8px;
  }

  .wrap {
    display: inline;
  }
  .card {
    margin: 20px;
    background-color: white;
    box-shadow: 1px 2px 6px;
    width: 32vh;
    height: 46vh;
    border-radius: 12px;
  }

  h3 {
    margin: 0;
  }

  img {
    border-radius: 12px;
  }
</style>
