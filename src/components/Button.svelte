<script>
    export let style = 'primary'
    export let type = 'button'
    export let disabled = false
  </script>
  
  <button {type} {disabled} class={style}>
    <slot></slot>
  </button>
  
  
  <style>
    button {
      border: 0;
      border-radius: 20px;
      width: max-content;
      padding: 10px;
      height: 40px;
      cursor: pointer;
      font-weight: 700;
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
      transform:scale(1);
      opacity: 1;
    }
  </style>