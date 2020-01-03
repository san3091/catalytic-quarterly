<script>
  import { windowOpen } from './store.js'
  export let title;
  export let light;
  export let buttonDisabled;

  // box-shadow: 5px 5px 5px #c2c2c2;
  const colorMode = light ? "light" : "dark"

  function closeWindow() {
    windowOpen.set(null)
  }
</script>

<div class="{`terminal_window terminal_window-${colorMode}`}">
  <div class="terminal_header">
    <button class="terminal_button terminal_button-red" disabled={buttonDisabled} on:click={closeWindow}></button>
    <h1 class="terminal_title">{title}</h1>
  </div>
  <slot></slot>
</div>

<style>
  .terminal_window {
    overflow: hidden;
    border-radius: 6px;
    height: 100%;
  }

  .terminal_window-dark {
    background-color: #2b2b2b;
  }

  .terminal_window-light {
    background-color: #fff;
  }

  .terminal_header {
    display: flex;
    flex-direction: row;
    justify-content: flex-start;
    align-items: center;
    background-color: #e6e6e6;
    height: 25px;
  }

  .terminal_title {
    color: black;
    font-size: 15px;
    margin: 0;
    margin-left: 15px;
  }

  .terminal_button {
    margin: 0;
    padding: 0;
    height: 12px;
    width: 12px;
    margin-left: 10px;
    border-radius: 10px;
  }

  .terminal_button:disabled {
    background-color: grey;
  }

  .terminal_button-red {
    background-color: #de4d40;
  }

  .terminal_content {
    overflow: scroll;
    color: white;
    font-size: 18px;
    margin: 18px;
    margin-bottom: 30px;
    height: 90%;
  }

  .terminal_window-dark .terminal_content {
    color: #fff;
  }

  .terminal_window-light .terminal_content {
    color: black;
  }
  
</style>
