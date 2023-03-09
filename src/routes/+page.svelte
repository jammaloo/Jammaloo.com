<script>
	import Picture from '../Picture.svelte';
	const headshot = 'headshot.jpg';
	const eyeball = 'eyeball.png';
	const resumePdf = 'James Freeman Resume.pdf';
	const resumeImg = 'resume.png';
	const ciImg = 'ci.png';
	const githubImg = 'github.png';
</script>

<div class="pictures">
	<Picture>
		<h1>James Freeman</h1>
	</Picture>

	<Picture padding={false}>
		<img src={headshot} alt="James Freeman's Headshot" />
	</Picture>

	<Picture>
		<p>
			<a href="https://blog.apollo350.com/posts/easy-ci-cd-with-github-actions">
				<img src={ciImg} alt="Thumbnail of a CI yaml file" />
				<span> Easy CI/CD with Github Actions </span>
			</a>
		</p>
	</Picture>

	<Picture>
		<a href="https://github.com/jammaloo">
			<img src={githubImg} alt="James' Github Profile" class="logo" />
		</a>
	</Picture>

	<Picture>
		<a href={resumePdf}>
			<img src={resumeImg} alt="A thumbnail of a resume" />
			<span> My Résumé </span>
		</a>
	</Picture>

	<Picture>
		<p>
			<a href="https://blog.apollo350.com/posts/video-calls-in-the-time-of-covid">
				<img
					src="https://blog.apollo350.com/assets/video-calls-in-the-time-of-covid/infrastructure.png"
					alt="A diagram of the infrastructure for video calls in the time of covid"
				/>
				<span> Video Calls in the Time of Covid </span>
			</a>
		</p>
	</Picture>

	<Picture padding={false}>
		<iframe
			title="James's Face that follows the cursor around, like some kind of horrible worm"
			src="https://jammaloo.com/faces/"
		/>
	</Picture>

	<Picture>
		<a href="https://jammaloo.com/random/EyeSeeYou/dist/">
			<img src={eyeball} alt="A colourful eyeball" />
		</a>
	</Picture>
</div>

<style>
	iframe {
		border: none;
		width: 50vw;
		height: 50vh;
	}

	img {
		max-width: 15vw;
	}

	.pictures {
		display: flex;
		flex-direction: row;
		align-items: center;
		justify-content: center;
		flex-wrap: wrap;
		gap: 1em;
	}

	a {
		text-align: center;
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		gap: 1em;
		font-size: 1.5em;
		color: var(--dark);
	}

	a img {
		display: block;
	}

	.logo {
		width: 5vw;
	}
</style>
