<script>
    export let label = "Click me"; 
    export let type = "button";
    export let disabled = false;
    export let onClick = () => {};
  </script>
  
  <button 
    type={type} 
    on:click={onClick} 
    disabled={disabled}
    class="p-4 bg-purple-700 text-white rounded-full cursor-pointer w-1/2 text-center flex justify-center items-center disabled:bg-gray-300 disabled:cursor-not-allowed hover:enabled:bg-purple-900">
    {label}
  </button>