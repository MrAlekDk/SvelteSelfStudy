<script>
    let count = 0;
$: squared = count * count;

function increment(){
    count++;
}
</script>

<button on:click={increment}>
    Clicked {count} {count === 1 ? 'time' : 'times'}
</button>
<p>{count} squared is {squared}</p>