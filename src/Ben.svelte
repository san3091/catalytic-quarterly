<script>
  import Terminal from './Terminal.svelte'
  import SansTitle from './typography/SansTitle.svelte'
  import SansBody from './typography/SansBody.svelte'
</script>

<Terminal title="ben hall's mix">
  <article class="terminal_content">
    <SansTitle>Ben Hall's Mix:</SansTitle>
      <SansBody>
        marian anderson hear de lambs a crying
      </SansBody>
      <SansBody>
        sonny sharrock black woman
      </SansBody>
      <SansBody>
        david shire theme from the conversation
      </SansBody>
      <SansBody>
        marzette watts lonely woman
      </SansBody>
      <SansBody>
        abbey lincoln let up
      </SansBody>
      <SansBody>
        alice coltrane turiya and ramakrishna
      </SansBody>
      <SansBody>
        miles davis I see your face before mine (musings of miles mix)
      </SansBody>
      <SansBody>
        oscar brown brother where art thou (original mix)
      </SansBody>
      <SansBody>
        james brown forever suffering
      </SansBody>
      <SansBody>
        max roach where you there when they crucified my lord
      </SansBody>
      <SansBody>
        andy bey celestial blues
      </SansBody>
      <SansBody>
        last poets blessed are those who struggle
      </SansBody>
      <SansBody>
        georgia anne muldrow the birth of petey wheatstraw
      </SansBody>
      <SansBody>
        dilla waves
      </SansBody>
      <SansBody>
        original last poets the shalimar
      </SansBody>
      <SansBody>
        kain look out for the blue guerrilla
      </SansBody>
      <SansBody>
        ramp I just love you
      </SansBody>
      <SansBody>
        aswad back to africa
      </SansBody>
      <SansBody>
        abyssinians leggo beast
      </SansBody>
      <SansBody>
        tappa zukie jah is i guiding light
      </SansBody>
      <SansBody>
        jennifer lara I am in love
      </SansBody>
      <SansBody>
        the sapphires who do you love
      </SansBody>
      <SansBody>
        barbara lewis hello stranger
      </SansBody>
  </article>
</Terminal>
<div class="ben_image">
  <Terminal title="ben_albums.png">
    <img alt="album covers for ben's mix" src="./images/ben_mix.png"/>
  </Terminal>
</div>

<style>
  .ben_image {
    position: absolute;
    right: -330px;
    top: 70px;
    height: 800px;
    width: 450px;
  }

  img {
    height: 100%
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
