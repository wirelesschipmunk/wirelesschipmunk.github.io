<script>
	import TopBar from "../lib/TopBar.svelte";

	const projects = [
		{
			name: "Dumplings Yum!",
			repoLink: "https://github.com/wirelesschipmunk/dumplings-yum",
			siteLink: "https://wirelesschipmunk.com/dumplings-yum/",
			description:
				"A nice looking restuarant website for chinese food. I also have a svelte version."
		},

		{
			name: "Epic Trivia",
			repoLink: "https://github.com/wirelesschipmunk/epic-trivia",
			siteLink: "https://wirelesschipmunk.com/epic-trivia/",
			description:
				"Terrible triva ok design. I got the colors from the vscode theme Campfire Syntax made by Nicholas Morrison."
		},

		{
			name: "HackerType (so original name)",
			repoLink: "https://github.com/wirelesschipmunk/hacker-type",
			siteLink: "https://wirelesschipmunk.com/hacker-type/",
			description: "Small clone of HackerTyper.com. Missing some features."
		},

		{
			name: "Rock Paper Scissors",
			repoLink: "https://github.com/wirelesschipmunk/hacker-type",
			siteLink: "https://wirelesschipmunk.com/hacker-type/",
			description: "My first project! Arguably the best. I'm planning to add a computer version."
		}
	];
</script>

<TopBar />

<h1 id="top">projects:</h1>

{#each projects as project}
	<div>
		<h1>{project.name}</h1>
		<h2>repo: <a href={project.repoLink}>{project.repoLink}</a></h2>
		<h2>site: <a href={project.siteLink}>{project.siteLink}</a></h2>
		<h4>{project.description}</h4>
	</div>
{/each}

<style>
	:global(body) {
		font-family: "Alpino", sans-serif;
		color: whitesmoke;
		background-color: rgb(28, 28, 28);
		padding: 0;
		margin: 0;
	}

	h1 {
		margin: 0.8em;
	}

	#top {
		margin-top: 4em;
	}

	div {
		margin-top: 4em;
		background-color: rgb(48, 48, 48);
		border-radius: 1em;
		padding: 0.6em;
		margin: 1em;
	}

	a {
		color: rebeccapurple;
	}
</style>
