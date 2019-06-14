<script>
	import Header from './Header.svelte';
	import Loginout from './Loginout.svelte';
	import Useful from './Useful.svelte';
	import Mousepos from './Mousepos.svelte';
	import Describe from './Describe.svelte';
	import Footer from './Footer.svelte';

	let count = 0;

	$: doubled = count * 2;
	$: quadrupled = doubled * 2;

	const handleClick = () => {
		count += 1;
	}

</script>

<!-- STYLE |||||||||||||||||||||||||||||||||||||||||||||| -->

<style>
	.container {
		font-size: 1.25rem;
		width: 60%;
		margin: 1em auto;
		padding: 1em;
	}

	@media screen and (max-width: 900px) {
		.container {
			width: 80%;
		}
	}

	@media screen and (max-width: 768px) {
		.container {
			width: 90%;
		}
	}
</style>

<!-- MARK UP |||||||||||||||||||||||||||||||||||||||||||| -->

<Header></Header>

<div class="container">

	Click Counter: 
	<button on:click={handleClick}>
		You Clicked {count} {count === 1 ? 'time' : 'times'}
	</button>

	<p>Double number of clicks is: {count} * 2 = {doubled}</p>
	<p>Quadrupled number of clicks is: {doubled} * 2 = {quadrupled}</p>

	<hr>

	Log In or Log Out: <Loginout></Loginout>

	<hr>

	<Useful></Useful>

	<hr>

	<Mousepos></Mousepos>

	<hr>

	<Describe></Describe>

</div>

<Footer></Footer>