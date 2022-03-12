<script>
    const ages ={
        alexander: "23 år",
        anders: "No clue xD",
        peter: "69 år",
        carsten: "33 år, dayum"
    };
    export let name;
    const age = ages[name.toLowerCase()]
</script>

<p>
	<span>The age for { name } is { age }</span>
</p>

<style>
	p {
		margin: 0.8em 0;
	}
	span {
		display: inline-block;
		padding: 0.2em 1em 0.3em;
		text-align: center;
		border-radius: 0.2em;
		background-color: #FFDFD3;
	}
</style>