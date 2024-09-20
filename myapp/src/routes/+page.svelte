<script>
	import Button from './Button.svelte';
	import Title from './Title.svelte';
	import Input from './Input.svelte';
  
	let inputValue = '';  // State to store input value
  
	function handleClick() {
	  alert('Button clicked!');
	}
  
	function handleInput(event) {
	  inputValue = event.target.value;
	  console.log("Input value: ", inputValue);
	}
  </script>
  
  <Title text="Svelte Component" />
  
  <h1 class="text-lg text-center mt-4">Add your email to find your account</h1>
  
  
  <Input value={inputValue} onInput={handleInput} placeholder="Enter Email" />
  
  
  <Button label="Log in" onClick={handleClick} />
  
  <svelte:head>
	<link rel="stylesheet" href="https://unpkg.com/tailwindcss@2.2.19/dist/tailwind.min.css" />
  </svelte:head>


