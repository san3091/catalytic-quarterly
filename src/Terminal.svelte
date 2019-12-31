<script>
  export let title;
</script>

<div class="terminal_window">
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
    background-color: #2b2b2b;
    width: 600px;
    height: 600px;
    overflow: hidden;
    border-radius: 6px;
    box-shadow: 5px 5px 5px #c2c2c2;
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
    color: white;
    font-size: 18px;
    margin: 18px;
  }
  
</style>
