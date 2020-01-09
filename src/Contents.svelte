<script>
  import Terminal from "./Terminal.svelte"
  import Ab from './Ab.svelte'
  import { windowOpen } from './store.js'

  let date = new Date()
  let image = 0

  const imageMap = {
    ab: "ab",
    ben: "ben",
    luke: "luke",
    elisabeth: "elisabeth",
    ig: "ig",
    ken: "ken",
    mats: "mats",
  }

  function updateBackground(title) {
    image = imageMap[title]
  }

  function updateWindowOpen(title) {
    windowOpen.set(title)
    // $: console.log($windowOpen)
  }

</script>

<div class="{`main_background ${image}`}">
  <div class="terminal_wrapper">
    <Terminal title="catalytic_quarterly #8 - january" buttonDisabled="true">
      <div class="terminal_content">
        <ul>
          <li><p>logged in: {date}</p></li> 
          <li><span 
                on:mouseenter={() => updateBackground("ab")} 
                on:click={() => updateWindowOpen("ab")} class="article article_ab">poor wheel - ab baars</span></li>
          <li><span 
                on:mouseenter={() => updateBackground("ben")} 
                on:click={() => updateWindowOpen("ben")} class="article article_ben">ben hall's mix</span></li>
          <li><span 
                on:mouseenter={() => updateBackground("luke")} 
                on:click={() => updateWindowOpen("luke")} class="article article_luke">feedback &amp; uplift: an interview with luke stewart - sam clapp</span></li>
          <li><span 
                on:mouseenter={() => updateBackground("elisabeth")} 
                on:click={() => updateWindowOpen("elisabeth")} class="article article_elisabeth">elisabeth harnik</span></li>
          <li><span 
                on:mouseenter={() => updateBackground("ig")} 
                on:click={() => updateWindowOpen("ig")} class="article article_ig">street chairs - ig henneman</span></li>
          <li><span 
                on:mouseenter={() => updateBackground("ken")} 
                on:click={() => updateWindowOpen("ken")} class="article article_ken">project notes for momentum five: stammer triptych, part two - ken vandermark</span></li>
          <li><span 
                on:mouseenter={() => updateBackground("mats")} 
                on:click={() => updateWindowOpen("mats")} class="article article_mats">WEAPON. JAZZ. SPONSORSHIP. - mats gustafsson</span></li>
        </ul>
      <div>
    </Terminal>
  </div>
</div>

<style>
  ul {
    list-style: none;
    padding: 0;
    margin: 0;
  }
  
  li {
    margin-bottom: 18px;
  }

  li:first-child {
    margin-bottom: 30px;
  }

  .terminal_content {
    background-color: #2b2b2b;
    color: white;
    font-size: 18px;
    padding: 18px;
    padding-bottom: 30px;
    height: 100%;
  }

  .main_background {
    width: 100%;
    height: 100vh;
    background-size: cover;
  }

  .ab {
    background-image: url('/images/background_1-glitched.png');
  }

  .ben {
    background-image: url('/images/background_2-glitched.png');
  }

  .luke {
    background-image: url('/images/background_3-glitched.png');
  }

  .ig {
    background-image: url('/images/background_4-glitched.png');
  }

  .elisabeth {
    background-image: url('/images/background_6-glitched.png');
  }

  .ken {
    background-image: url('/images/background_7-glitched.png');
  }

  .mats {
    background-image: url('/images/background_8-glitched.png');
  }

  .terminal_wrapper {
    position: absolute;
    top: 40px;
    left: 50px;
    width: 600px;
    height: 600px;
  }

  .article {
    color: white;
    text-decoration: underline;
    cursor: pointer;
  }

  .article:hover {
    color: black;
    background-color: white;
  }

  .article:hover::before {
    content: "> ";
  }
</style>
