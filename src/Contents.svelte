<script>
  import Terminal from "./Terminal.svelte"

  let date = new Date()
  let count = 0

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
  }
</script>

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
    <li>{count}</li>
  </ul>
</Terminal>

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
