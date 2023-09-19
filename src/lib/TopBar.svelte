<div>
	<img src="src/lib/images/slugcat-pfp.png" alt="slugcat-pfp" />

	<h1>wirelesschipmunk</h1>

	<button
		style="margin-left: auto;"
		on:click={() => (window.location = "https://github.com/wirelesschipmunk/")}>github!</button
	>
	<button>about!</button>
	<button>&#9775;</button>
	<button>&#9776;</button>
</div>

<style>
	div {
		display: flex;
		flex-direction: row;
		justify-content: space-between;
		align-items: center;
		gap: 0.5em;
		background-color: rgb(28, 28, 28);
		top: 0;
		width: 100%;
		position: fixed;
	}

	img {
		border-radius: 2em;
		width: 55px;
		box-shadow: 2px 2px 0px rebeccapurple;
		border: solid;
		border-color: gray;
		border-width: 1.85px;
		margin-left: 0.3em;
	}

	button {
		font: inherit;
		color: whitesmoke;
		background-color: rgb(55, 55, 55);
		border: solid;
		border-color: gray;
		border-width: 1.85px;
		border-radius: 10px;
		box-shadow: 2px 2px 0px rebeccapurple;
		padding: 0.6em 1.5em;
		margin-right: 0.3em;
		cursor: pointer;
		transition: all 0.15s;
	}

	button:active {
		background-color: rebeccapurple;
		box-shadow: 1px 1px 0px rebeccapurple;
		opacity: 0.8;
	}
</style>
