<script>
    let count = 0;

    function incrementCounter(){
        count++;
    }
</script>

<button on:click={incrementCounter}>
    Clicked {count} {count === 1 ? 'time' : 'times'} on the button
</button>