<script>
    let counter = 0;
    let x = 8;

    let user ={
        loggedIn: false
    };

    function toggle(){
        user.loggedIn = !user.loggedIn;
        counter++;
    }

</script>

{#if user.loggedIn}
	<button on:click={toggle}>
		Log out
	</button>
{/if}

{#if !user.loggedIn}
	<button on:click={toggle}>
		Log in
	</button>
{/if}

{#if counter>10}
	<p>Waow, you've pressed more than 10 times, gj</p>
{:else}
    <p>Keep pressing the button</p>
{/if}

{#if x > 10}
	<p>{x} is greater than 10</p>
{:else if 5 > x}
	<p>{x} is less than 5</p>
{:else}
	<p>{x} is between 5 and 10</p>
{/if}