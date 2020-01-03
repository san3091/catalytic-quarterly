<script>
  import Terminal from './Terminal.svelte'
  import TimesTitle from './TimesTitle.svelte'
  import TimesBody from './TimesBody.svelte'
</script>

<Terminal title="POOR WHEEL" light="true">
  <article class="terminal_content">
    <TimesTitle>POOR WHEEL</TimesTitle>
    <TimesBody>
      This month exactly 30 years ago I studied in Los Angeles with John Carter: clarinetist, composer and black belt aikido master. Very happy to return again to that city as part of my upcoming USA solo tour. Los Angeles the place where I experienced such an inspiring musical period in 1989 with John and also with his family.
    </TimesBody>
    <TimesBody>
      My tour will be from April 17 until May 11 travelling the country and play eighteen concerts. With such distances I thought the title Poor Wheel would be appropriate for this long trip. Pianist composer Misha Mengelberg, while driving home after a concert in the North of Holland, got a flat tire, replaced it with a small spare wheel and suffered the whole drive from a wheel that according to Misha ‘squeaked and cried softly.’ The beautiful ballad Poor Wheel was born.
    </TimesBody>
    <TimesBody>
      Since I first started making music I listened extensively to ballads that were being played by the great saxophonists and clarinetists in jazz history. These inspiring examples became part of my playing, my sound, my language. My most recent solo CD is a salute to that tradition. The compositions and improvisations were inspired by fine musicians like clarinetist John Carter, saxophonist John Coltrane and pianists, composers Duke Ellington, Misha Mengelberg, Carl T. Fischer, Oscar Levant and the wonderful shakuhachi player Watazumi Doso.
    </TimesBody>
    <TimesBody>
      The program for my tour is inspired by this solo CD entitled And She Speaks – A Collection of Ballads. Playing these ballads for the CD was very important to me because it seems that for the first time I really succeeded in bringing together compositions and improvisations in a natural way, that is: going in and out of the material, going in and out of the tradition, to incorporate my own language in these ballads that I have known so long already. Finally I made them mine. And She Speaks is a ballad written by John Carter.
    </TimesBody>
    <TimesBody>
      The beautiful memories of warm, dedicated and inspiring audiences in the USA I experienced during earlier tours… I am looking forward to it.
    </TimesBody>
    <TimesBody>
      Hope to meet many USA music lovers and fans again. I will bring my tenor sax, clarinet and shakuhachi: the Japanese bamboo.
    </TimesBody>
    <TimesBody>
      Hereby the itinerary: New York, Boston, Buffalo, Cleveland, Chicago, Seattle, Portland, Los Angeles, Flagstaff, Shreveport, New Orleans, Columbia, Philadelphia
    </TimesBody>
    <TimesBody>
      For more information: www.stichtingwig.com
    </TimesBody>
  </article>
</Terminal>
<div class="ab_image">
  <Terminal title="AbPhoto_CQ8.jpg">
    <img alt="ab" src="./images/AbPhoto_CQ8.jpg" />
  </Terminal>
</div>

<style>

  .ab_image {
    position: absolute;
    left: -340px;
    bottom: -100px;;
    height: 500px;
    width: 300px;
  }

  img {
    width: 100%;
  }

  .terminal_content {
    background-color: white;
    color: #00c900;
    overflow: scroll;
    font-size: 18px;
    padding: 18px;
    padding-bottom: 30px;
    height: 100%;
  }

</style>
