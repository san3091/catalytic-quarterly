<script>
  import Terminal from './Terminal.svelte'
  import SansBody from './typography/SansBody.svelte'
</script>

<Terminal title="IG_images_CQ8.zip">
  <article class="terminal_content">
    <img src="./images/vancouver.jpg"/>
    <img src="./images/kultur.jpg"/>
    <img src="./images/amsterdam.jpg"/>
    <img src="./images/guelph.jpg"/>
    <img src="./images/studio.jpg"/>
  </article>
</Terminal>
<div class="text">
  <Terminal title="street chairs - ig henneman">
    <article class="terminal_content">
      <SansBody>Street chairs – uncertain future</SansBody>
      <SansBody>
        a chair is a piece <br/>
        of furniture <br/>
        raised surface <br/>
        supported <br/>
        by legs commonly used <br/>
        to seat <br/>
        a single person <br/>
      </SansBody>
      <SansBody>
        a chair is a piece <br/>
        of furniture <br/>
        raised surface <br/>
        supported <br/>
        by legs commonly used <br/>
        to seat <br/>
        a single person <br/>
      </SansBody>
      <SansBody>
        1. East 4th Ave Vancouver <br/>
        2. Kulturforum Villach<br/>
        3. Kerkstraat Amsterdam<br/>
        4. Jane St Guelph <br/>
        5. Prinsengracht Amsterdam<br/>
      </SansBody>
    </article>
  </Terminal>
</div>

<style>
  .text {
    position: absolute;
    top: 120px;
    right: -200px;
    width: 300px;
    height: 600px;
  }

  img {
    width: 100%;
  }

  .terminal_content {
    background-color: #fff;
    color: #223d2a;
    overflow: scroll;
    font-size: 18px;
    font-weight: 700;
    padding: 0 18px;
    padding-bottom: 30px;
    height: 95%;
  }
</style>


