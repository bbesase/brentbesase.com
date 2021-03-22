<script>
	export let cardType = "";
</script>

<svelte:head>
	<link rel="preconnect" href="https://fonts.gstatic.com" />
	<link
		href="https://fonts.googleapis.com/css2?family=Indie+Flower&family=Lato&family=Oswald&display=swap"
		rel="stylesheet"
	/>
</svelte:head>

<div class="container-fluid">
	<div
		class="col-lg-6 col-lg-offset-0 col-md-6 col-md-offset-0 col-sm-10 col-sm-offset-1 col-xs-12"
	>
		<figure>
			<div
				class="media"
				style="background-image:url(https://s3-us-west-2.amazonaws.com/s.cdpn.io/584938/bg_15.png)"
			/>
			<!-- svelte-ignore a11y-structure -->
			<div class="text-container">
				<svg
					viewBox="0 0 200 200"
					version="1.1"
					preserveAspectRatio="none"
					xmlns="http://www.w3.org/2000/svg"
				>
					<defs>
						<mask id="mask" x="0" y="0" width="100%" height="100%">
							<rect id="alpha" x="0" y="0" width="100%" height="100%" />
								<text
									class="title"
									dx="50%"
									dy="2.5em">ENJOY
								</text>
								<!-- <text class="title" dx="50%" dy="3.5em">EVERY</text>
								<text
									class="title"
									dx="50%"
									dy="4.5em">MOMENT
								</text> -->
						</mask>
					</defs>
					<rect id="base" x="0" y="0" width="100%" height="100%" />
				</svg>
				<div class="text">
					<p>
						Enamel pin selvage health goth edison bulb, venmo glossier tattooed
						hella butcher cred iPhone.
					</p>
				</div>
			</div>
			<a href="#" />
		</figure>
	</div>
	<!-- <div class="col-lg-6 col-md-6 hidden-sm hidden-xs">
		<figure>
			<div
				class="media"
				style="background-image:url(https://s3-us-west-2.amazonaws.com/s.cdpn.io/584938/bg_5.png)"
			/>
			<figcaption>
				<svg
					viewBox="0 0 200 200"
					version="1.1"
					preserveAspectRatio="none"
					xmlns="http://www.w3.org/2000/svg"
				>
					<defs>
						<mask id="mask" x="0" y="0" width="100%" height="100%">
							<rect id="alpha" x="0" y="0" width="100%" height="100%" />
							<text
								class="title"
								dx="50%"
								dy="2.5em">ENJOY</text
							>
							<text class="title" dx="50%" dy="3.5em">EVERY</text>
							<text
								class="title"
								dx="50%"
								dy="4.5em">MOMENT
							</text>
						</mask>
					</defs>
					<rect id="base" x="0" y="0" width="100%" height="100%" />
				</svg>
				<div class="body">
					<p>
						Enamel pin selvage health goth edison bulb, venmo glossier tattooed
						hella butcher cred iPhone. Plaid skateboard man braid wayfarers.
					</p>
				</div>
			</figcaption>
			<a href="#" />
		</figure>
	</div> -->
</div>

<style>
	.container-fluid {
	 width: 100%;
}
 .media {
	 background-position: center;
	 background-size: cover;
	 height: 100%;
	 position: absolute;
	 transition: all 0.3s ease;
	 width: 100%;
}
 figure {
	 height: 370px;
	 overflow: hidden;
	 position: relative;
}
 figure a {
	 height: 100%;
	 left: 0;
	 position: absolute;
	 top: 0;
	 width: 100%;
	 z-index: 3;
}
 figure:hover .media {
	 transform: scale(1.25);
}
 .text-container {
	 color: rgb(65,65,65);
	 height: calc(100% - 30px);
	 margin: 15px;
	 left: 0;
	 position: absolute;
	 top: 0;
	 width: 250px;
}
 .text {
	 background-color: white;
	 bottom: 0;
	 padding: 15px;
	 position: absolute;
}
 svg {
	 height: inherit;
	 width: 100%;
}
 svg text {
	 text-anchor: middle;
}
 svg #alpha {
	 fill: white;
}
 svg .title {
	 /* font-size: 28px;
	 font-family: "Montserrat"; */
	 font-size: 40px;
	 font-family: 'Indie Flower', cursive;
	 letter-spacing: 5px;
}
 svg #base {
	 fill: white;
	 -webkit-mask: url(#mask);
	 mask: url(#mask);
}
</style>
