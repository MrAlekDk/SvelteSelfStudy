<script>
	export let name;
	import Introduction from "./components/introduction/introduction.svelte"
	import Reactivity from "./components/reactivity/Reactivity.svelte"
	import Props from "./components/Props/Props.svelte"
	import Logic from "./components/Logic/Logic.svelte"
	import Events from "./components/Events/Events.svelte"
</script>

<main>
	<h1>Hello {name}!</h1>
	<div class="box">
		<Introduction/>
	</div>
	<div class="box">
		<Reactivity />
	</div>
	<div class="box">
		<Props />
	</div>
	<div class="box">
		<Logic />
	</div>
	<div class="box">
		<Events />
	</div>


</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	.box{
		border : solid 1px black;
	}


	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}



	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>