<script>
  import Terminal from './Terminal.svelte'
  import TimesTitle from './typography/TimesTitle.svelte'
  import TimesBody from './typography/TimesBody.svelte'
</script>

<div class="ken_image">
  <Terminal title="personnel_stammer-photos">
    <img alt="album covers for ben's mix" src="./images/ben_mix.png"/>
  </Terminal>
</div>

<Terminal title="ben hall's mix">
  <article class="terminal_content">
  </article>
</Terminal>

<style>
  .ken_image {
    position: absolute;
    right: -330px;
    top: 70px;
    height: 800px;
    width: 450px;
  }

  img {
    height: 100%;
  }

  .terminal_content {
    background-color: white;
    overflow: scroll;
    font-size: 16px;
    line-height: 11px;
    padding: 18px;
    padding-bottom: 30px;
    height: 100%;
  }

</style>
