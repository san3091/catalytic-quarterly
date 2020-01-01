<script>
  export let title;
  export let light;

  // box-shadow: 5px 5px 5px #c2c2c2;
  const colorMode = light ? "light" : "dark"
</script>

<div class="{`terminal_window terminal_window-${colorMode}`}">
  <div class="terminal_header">
    <div class="terminal_button terminal_button-red"></div>
    <h1 class="terminal_title">{title}</h1>
  </div>
  <div class="terminal_content">
    <slot></slot>
  </div>
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
    height: 12px;
    width: 12px;
    margin-left: 10px;
    border-radius: 10px;
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
