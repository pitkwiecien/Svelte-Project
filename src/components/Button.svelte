<script>
  export let style = 'primary'
  export let type = 'button'
  export let disabled = false
  export let fontSize = 1;
</script>
  
  <button {type} {disabled} class={style} style="--font-size: {fontSize}">
    <slot></slot>
  </button>
  
  
  <style>
    button {
      font-size: 1em;
      border: 0;
      padding: 20px;
      border-radius: 20em;
      cursor: pointer;
      font-weight: 700;
      width: max-content;
    }

    .primary {
      background-color: #ff4444;
      color: #fff;
    }

    .secondary {
      background-color: #fff;
      color: #ff4444;
    }
    button:hover {
      transform: scale(0.98);
      opacity: 0.9;
    }
    button:disabled{
      background-color: #cccccc;
      color: #333;
      cursor:auto;
    }
    button:disabled:hover{
      transform: scale(1);
      opacity: 1;
    }
  </style>