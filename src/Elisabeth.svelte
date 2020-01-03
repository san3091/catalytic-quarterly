<script>
  import Terminal from './Terminal.svelte'
  import SansBody from './typography/SansBody.svelte'
</script>

<Terminal title="G_4235.jpg">
  <img alt="waldklavier" src="./images/waldklavier.png"/>
</Terminal>
<div class="text">
<Terminal title="elisabeth waldklavier">
  <article class="terminal_content">
    <SansBody>
The 'Waldklavier' (forest piano) - a discarded old grand piano from the family property of a friend - was first played in 2014 as part of an audiovisual outdoor performance (Harnik/Kern/Richter) at the Kunsthaltestelle Streckhammerhaus in Frohnleiten/Austria. In 2015, the grand piano was part of the collaborative installation 'articulations in space' (Harnik/Richter/Thon) at Rhizom Graz/Austria and has since inhabited the forest of Pairidaeza near Graz at the invitation of Manfred Kummer. In the spring of the following year, I visited the piano for the first time after the exhibition and set out in search of the starting point of its ‘instrumentality,' i.e. the sound of the natural material combination wood-metal, and investigated the traces of sound the story had left behind.
    </SansBody>
    <SansBody>
I was interested in the 'total' of the sound image, i.e. the 'undivided' overall sound that is transferred to the soundboard when the body is struck at different points with a rubber hammer. The strings released from the dampers reacted very subtly to every change of touch and the soundboard amplified the quiet echoes of the past in a complex and uncontrolled way. The sound recordings I made, created in this almost animistic way of approaching the instrument, were played as an installation during the Architecture Summer 2018 via a transducer attached to the soundboard of the piano in the forest of Pairidaeza. 
    </SansBody>
    <SansBody>
Can you imagine its sounds?
    </SansBody>
  </article>
</Terminal>
</div>

<style>
  img {
    height: 100%;
  }

  .text {
    position: absolute;
    top: -130px;
    right: -280px;
    width: 400px;
    height: 630px;
  }

  .terminal_content {
    background-color: black;
    color: white;
    overflow: scroll;
    font-size: 15px;
    line-height: 17px;
    padding: 18px;
    padding-bottom: 30px;
    height: 100%;
  }
</style>
