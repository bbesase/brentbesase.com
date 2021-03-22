<script>
	export let segment;
</script>

<style>
	nav {
		font-weight: 300;
		padding: 0 1em;
		height: 10vh;
	}

	ul {
		margin: 0;
		padding: 0 10vw 0 0;
		display: flex;
    justify-content: flex-end;
		height: 100%;
		align-items: center;
	}

	/* clearfix */
	ul::after {
		content: '';
		display: block;
		clear: both;
	}

	li {
		display: block;
		float: right;
	}

	[aria-current] {
		position: relative;
		display: inline-block;
	}

	[aria-current]::after {
		position: absolute;
		content: '';
		width: calc(100% - 1em);
		height: 2px;
		background-color: rgb(237,237,237);
		display: block;
		bottom: -2px;
	}

	a {
		text-decoration: none;
		padding: 1em 0.5em;
		display: block;
		color: rgb(237,237,237);
		font-size: 20px;
		font-family: 'Indie Flower', cursive;
	}
</style>

<nav>
	<ul>
		<li><a aria-current="{segment === undefined ? 'page' : undefined}" href=".">Home</a></li>
		<li><a aria-current="{segment === 'about' ? 'page' : undefined}" href="about">About</a></li>
		<li><a aria-current="{segment === 'skillset' ? 'page' : undefined}" href="skillset">Skill Set</a></li>
		<li><a aria-current="{segment === 'contact' ? 'page' : undefined}" href="contact">Contact</a></li>


		<!-- for the blog link, we're using rel=prefetch so that Sapper prefetches
		     the blog data when we hover over the link or tap it on a touchscreen -->
		<!-- <li><a rel=prefetch aria-current="{segment === 'blog' ? 'page' : undefined}" href="blog">blog</a></li> -->
	</ul>
</nav>
