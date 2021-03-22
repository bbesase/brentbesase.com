<svelte:head>
  <link rel="preconnect" href="https://fonts.gstatic.com">
	<link href="https://fonts.googleapis.com/css2?family=Indie+Flower&family=Lato&family=Oswald&display=swap" rel="stylesheet">
</svelte:head>

<script>
  export let text = '';
</script>

<div>{text}</div>

<style>
  div {
    font-family: 'Indie Flower', cursive;
    color: rgb(237,237,237);
    font-size: 4vh;
    text-shadow: 1px 1px 1px rgba(0, 0, 0, 0.45);
    display: flex;
    justify-content: center;
    align-items: center;
  }
  div::before, div::after {
    content: '';
    display: block;
    height: 0.09em;
    min-width: 30vw;
  }
  div::before {
    background: linear-gradient(to right, rgba(240, 240, 240, 0), rgb(237,237,237));
    margin-right: 4vh;
  }
  div::after {
    background: linear-gradient(to left, rgba(240, 240, 240, 0), rgb(237,237,237));
    margin-left: 4vh;
  }
</style>