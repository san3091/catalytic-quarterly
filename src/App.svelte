<script>
  import Contents from './Contents.svelte'
  import Ab from './Ab.svelte'
  import Ben from './Ben.svelte'
  import Luke from './Luke.svelte'
  import Elisabeth from './Elisabeth.svelte'
  import Ig from './Ig.svelte'
  import { windowOpen } from './store.js'
</script>

<svelte:head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
  <title>Catalytic Sound Quarterly #8</title>

  <meta property="og:url"                content="https://catalyticsound.com/quarterly/8" />
  <meta property="og:type"               content="article" />
  <meta property="og:title"              content="Catalytic Sound Quarterly #8" />
  <meta property="og:description"        content="Catalytic Sound Newsletter - January 2020" />
  <meta property="og:image"              content="http://catalyticsound.com/quarterly/8/fbmeta.jpg" />
  <meta property="og:image:width"        content="1920px" />
  <meta property="og:image:height"       content="1080px" />

  <meta name="twitter:card" content="summary">
  <meta name="twitter:site" content="@kenvandermark">
  <meta name="twitter:url" content="https://catalyticsound.com/quarterly/8">
  <meta name="twitter:title" content="Catalytic Sound Quarterly #8">
  <meta name="twitter:description" content="Catalytic Sound Newsletter - January 2019">
  <link href="https://fonts.googleapis.com/css?family=Cutive+Mono&display=swap" rel="stylesheet">
  <meta name="author" content="Catalytic Sound">
</svelte:head>

<main>
  <Contents />
  {#if $windowOpen === "ab"}
    <section class="ab_window">
      <Ab />
    </section>
  {:else if $windowOpen === "ben"}
    <section class="ben_window">
      <Ben />
    </section>
  {:else if $windowOpen === "luke"}
    <section class="luke_window">
      <Luke />
    </section>
  {:else if $windowOpen === "elisabeth"}
    <section class="elisabeth_window">
      <Elisabeth />
    </section>
  {:else if $windowOpen === "ig"}
    <section class="ig_window">
      <Ig />
    </section>
  {/if}
</main>

<style>
  :global(body) {
    padding: 0;
  }

	main {
		max-width: 240px;
    font-family: 'Cutive Mono', 'andale mono';
	}

  .ab_window {
    position: absolute;
    top: 110px;
    left: 420px;
    width: 900px;
    height: 700px;
  }

  .ben_window {
    position: absolute;
    top: 10px;
    left: 300px;
    width: 600px;
    height: 800px;
  }

  .luke_window {
    position: absolute;
    top: 90px;
    left: 200px;
    width: 1000px;
    height: 800px;
  }

  .elisabeth_window {
    position: absolute;
    top: 140px;
    left: 160px;
    width: 900px;
    height: 700px;
  }

  .ig_window {
    position: absolute;
    top: 70px;
    left: 300px;
    width: 800px;
    height: 800px;
  }

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>
