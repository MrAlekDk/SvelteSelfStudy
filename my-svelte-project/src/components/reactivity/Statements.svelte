<script>
	let count = 0;

	function handleClick() {
		count += 1;
	}

    $: {
	console.log('the count is ' + count);
}

$: if (count >= 10) {
    count++;
	alert('count is higher than 10, puttin it back to 0');
	count = 0;
}
</script>

<button on:click={handleClick}>
	Clicked {count} {count === 1 ? 'time' : 'times'}
</button>