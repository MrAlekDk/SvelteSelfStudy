<script>

    let color = "green"
    function clickHandler(){
        console.log("Switch")
        color = "red"
    }
</script>

<h1 style="color:{color};">I am a single button, wink wink</h1>

<button on:click|once={clickHandler}>Click me</button>
