<script lang="ts">
	// You can add props to make this component more dynamic
	export let title = 'Card Title';
	export let bodyText =
		'This is some content inside the card. It can be anything you want - text, images, links, etc.';
	export let buttonText = 'Click Me';
	function handleButtonClick() {
		console.log('Button clicked!');
	}
</script>

<div class="card">
	<div class="card-header">
		{title}
	</div>
	<div class="card-body">
		{bodyText}
	</div>
	<div class="card-footer">
		<button on:click={handleButtonClick}>{buttonText}</button>
	</div>
</div>

<style>
	.card {
		background-color: white;
		border: 1px solid #ccc;
		border-radius: 8px;
		box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
		margin: 20px;
		padding: 20px;
		width: 300px;
	}
	.card-header {
		font-size: 1.5em;
		margin-bottom: 20px;
	}
	.card-body {
		margin-bottom: 20px;
	}
	.card-footer {
		text-align: right;
	}
	button {
		background-color: #007bff;
		border: none;
		border-radius: 5px;
		color: white;
		cursor: pointer;
		padding: 10px 20px;
	}
	button:hover {
		background-color: #0056b3;
	}
</style>
