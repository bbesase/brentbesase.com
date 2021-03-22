<script>
	import Divider from '../components/Divider.svelte';
	import Card from '../components/Card.svelte';

	const heart = '<3';
</script>

<svelte:head>
	<link rel="preconnect" href="https://fonts.gstatic.com">
	<link href="https://fonts.googleapis.com/css2?family=Indie+Flower&family=Lato&family=Oswald&display=swap" rel="stylesheet">

	<title>About</title>
</svelte:head>

<p class="header">About Me</p>

<div class="section">
	<Divider text={'Origin Story'}/>

	<div class="origins">
		I'm just a city boy, born and raised South of Detroit [Toledo, OH] I grew up playing just about every sport and video game possible until I finally decided on some to stick with.
		I attended the University of Toledo pursuing a bachelors degree in Computer Science Engineering. I was always drawn to the beach as a kid, so once I got my degree, I decided to pack my bags
		up, and make a giant leap of faith and move to Raleigh, NC. A place where I now call home {heart}
	</div>

	<Divider text={'Hobbies'}/>

	<Card />
</div>

<style>
	.header {
		font-size: 60px;
		font-family: 'Indie Flower', cursive;
		font-weight: 400;
	}

	.origins {
		font-size: 30px;
		font-family: 'Oswald', sans-serif;
		font-weight: 200;
	}
</style>