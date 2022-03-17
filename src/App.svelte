<script>
  import Album from "./Album.svelte";
  import Footer from "./Footer.svelte";
  import Button from "./Button.svelte";
  import Badge from "./Badge.svelte";
  import Card from "./Card.svelte";
  import Buttonbadge from "./Buttonbadge.svelte";
</script>

<h1>Designsystem ==> Kode</h1>

<main>
  <div class="badge_container">
    <h2>Badges</h2>
    <div class="badge_bar">
      <Badge>Default</Badge>
      <Badge type="primary">Primary</Badge>
      <Badge type="secondary">Secondary</Badge>
      <Badge type="accent">Accent</Badge>
      <Badge type="ghost">Ghost</Badge>
    </div>
  </div>

  <div class="button_container">
    <h2>Buttons</h2>
    <div class="button_bar">
      <Button>Default</Button>
      <Button type="primary">Primary</Button>
      <Button type="primary" mode="inversed">Primary inversed</Button>
      <Button type="secondary">Secondary</Button>
      <Button type="secondary" mode="inversed">Secondary inversed</Button>
      <Button type="accent">Accent</Button>
      <Button type="accent" mode="inversed">Accent inversed</Button>
      <Button type="ghost">Ghost</Button>
      <Button type="link">Link</Button>
    </div>
  </div>

  <h2>Cards</h2>
  <div class="card_container">
    <Card description="Fine sko, meget nye og aldrig brugs før" product="Sko"
      >Nike airforce one</Card
    >
    <Card
      description="Grimme sko med mange ridser, mudder klatter og diverse uidentificerede pletter"
      product="Sko">Vans old skool</Card
    >
  </div>

  <h2>Button with badge component</h2>
  <Buttonbadge />
</main>

<Footer />

<style>
  main {
    text-align: center;
    padding: 1em;
  }

  .button_container {
    display: block;
  }
  .button_bar {
    display: inline-flex;
    flex-direction: row;
    flex-flow: row;
    justify-content: space-evenly;
    margin-top: 15px;
  }
  .badge_container {
    display: block;
  }

  .badge_bar {
    display: inline-flex;
    flex-direction: row;
    flex-flow: row;
    justify-content: space-evenly;
  }
  .card_container {
    margin-left: 20vw;
    margin-right: 20vw;
    display: grid;
    justify-content: center;
  }
</style>
