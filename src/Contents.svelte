<script>
  import Terminal from "./Terminal.svelte"
  import Ab from './Ab.svelte'

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
</script>

<div class="{`main_background ${image}`}">
  <div class="terminal_wrapper">
    <Terminal title="catalytic_quarterly #8 - january">
      <ul>
        <li><p>logged in: {date}</p></li> 
        <li><span on:mouseenter={() => updateBackground("ab")} class="article article_ab">poor wheel - ab baars</span></li>
        <li><span on:mouseenter={() => updateBackground("ben")} class="article article_ben">ben hall's mix</span></li>
        <li><span on:mouseenter={() => updateBackground("luke")} class="article article_luke">feedback & uplift: an interview with luke stewart - sam clapp</span></li>
        <li><span on:mouseenter={() => updateBackground("elisabeth")} class="article article_elisabeth">elisabeth harnik</span></li>
        <li><span on:mouseenter={() => updateBackground("ig")} class="article article_ig">street chairs - ig henneman</span></li>
        <li><span on:mouseenter={() => updateBackground("ken")} class="article article_ken">project notes for momentum five: stammer triptych, part two - ken vandermark</span></li>
        <li><span on:mouseenter={() => updateBackground("mats")} class="article article_mats">WEAPON. JAZZ. SPONSORSHIP. - mats gustafsson</span></li>
      </ul>
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

  .main_background {
    width: 100%;
    height: 100vh;
    background-size: cover;
  }

  .ab {
    background-image: url('/images/blue_saturated.png');
  }

  .ben {
    background-image: url('/images/grey_broken.png');
  }

  .luke {
    background-image: url('/images/green_saturated.png');
  }

  .ig {
    background-image: url('/images/orange_broken.png');
  }

  .elisabeth {
    background-image: url('/images/music_broken.png');
  }

  .ken {
    background-image: url('/images/text_broken.png');
  }

  .mats {
    background-image: url('/images/chair_broken.png');
  }

  .terminal_wrapper {
    background-color: black;
    margin: 40px 70px;
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
