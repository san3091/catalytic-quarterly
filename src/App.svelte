<script>
  import Contents from './Contents.svelte'
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
  <div class="terminal_wrapper">
    <Contents />
  </div>
</main>

<style>
	main {
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
    font-family: 'Cutive Mono', 'andale mono';
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>
