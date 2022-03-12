<script>
    let letters = ['a', 'b', 'c', 'd'];


    function addLetter(){
        letters.push(String.fromCharCode(letters.length+97));
        letters = letters;
    }

    function removeLetter(){
        letters.pop();
        letters=letters;
    }

</script>

<p>{letters.join()}</p>

<button on:click={addLetter}>
	Add a letter
</button>
<button on:click={removeLetter}>
	Remove a letter
</button>