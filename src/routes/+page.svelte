<script>
	import TopBar from "../lib/TopBar.svelte";
	import dumplingsYumImg from "../lib/images/dumplings-yum.png";
	import epicTriviaImg from "../lib/images/epic-trivia.png";
	import hackerTypeImg from "../lib/images/hacker-type.png";
	import rockPaperScissorsImg from "../lib/images/rock-paper-scissors.png";

	const projects = [
		{
			name: "Dumplings Yum!",
			repoLink: "https://github.com/wirelesschipmunk/dumplings-yum",
			siteLink: "https://wirelesschipmunk.com/dumplings-yum/",
			description:
				"A nice looking restuarant website for chinese food. I also have a svelte version.",
			img: dumplingsYumImg
		},

		{
			name: "Epic Trivia",
			repoLink: "https://github.com/wirelesschipmunk/epic-trivia",
			siteLink: "https://wirelesschipmunk.com/epic-trivia/",
			description:
				"Pretty terrible triva, ok design. I got the colors from the vscode theme Campfire Syntax made by Nicholas Morrison.",
			img: epicTriviaImg
		},

		{
			name: "HackerType (so original name)",
			repoLink: "https://github.com/wirelesschipmunk/hacker-type",
			siteLink: "https://wirelesschipmunk.com/hacker-type/",
			description: "Small clone of HackerTyper.com. Missing some features.",
			img: hackerTypeImg
		},

		{
			name: "Rock Paper Scissors",
			repoLink: "https://github.com/wirelesschipmunk/rock-paper-scissors",
			siteLink: "https://wirelesschipmunk.com/Rock-Paper-Scissors/",
			description: "My first project! Arguably the best. I'm planning to add a computer version.",
			img: rockPaperScissorsImg
		}
	];
</script>

<TopBar />

<h1 id="top">projects:</h1>

{#each projects as project}
	<div>
		<div>
			<h1>#{project.name}</h1>
			<h3>{project.description}</h3>
			<h2>repo: <a href={project.repoLink} target="_blank">{project.repoLink}</a></h2>
			<h2>site: <a href={project.siteLink} target="_blank">{project.siteLink}</a></h2>
		</div>
		<img src={project.img} />
	</div>
{/each}

<h1 id="top">about</h1>
<h3>
	Hi! My name is <span style="color: rebeccapurple;">undefined null syntax error the third</span>
	and I'm a 13 year old web developer (obviusly). I've been learning
	<span style="color: rgb(232, 193, 0);">JavaScript</span>/<span style="color: red;">HTML</span
	>/<span style="color: aqua;">CSS</span>
	for about 4 months and I just started learning (and using)
	<span style="color: rgb(224, 71, 0);">Svelte.</span>
</h3>

<p>made with <span style="color: rgb(224, 71, 0);">Svelte!</span></p>

<style>
	:global(body) {
		font-family: "Alpino", sans-serif;
		color: whitesmoke;
		background-color: rgb(28, 28, 28);
		padding: 0;
		margin: 0;
	}

	h1 {
		margin: 0.6em;
		width: 300px;
	}

	h3 {
		margin: 0.4em;
		margin-bottom: 5em;
	}

	#top {
		margin-top: 4em;
	}

	div {
		display: flex;
		flex-direction: row;
		justify-content: space-between;
		margin-top: 4em;
		background-color: rgb(48, 48, 48);
		border-radius: 1em;
		padding: 0.6em;
		margin: 1em;
	}

	div div {
		display: flex;
		flex-direction: column;
	}

	img {
		height: 500px;
		border-radius: 1em;
	}

	a {
		color: rebeccapurple;
		width: 200px;
	}
</style>
