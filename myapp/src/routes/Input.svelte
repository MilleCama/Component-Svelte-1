<script>
  export let value = "";  
  export let placeholder = "Enter text"; 
  export let disabled = false;
  export let onInput = (event) => {};
</script>

<input 
  bind:value={value}  
  placeholder={placeholder}
  disabled={disabled}
  on:input={onInput} 
  class="p-2 border border-white-500 rounded-md text-base w-full disabled:bg-gray-200"
/>