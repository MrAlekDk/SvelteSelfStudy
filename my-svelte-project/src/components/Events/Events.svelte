<script>
    import MouseEx from "./Mouse.svelte"
    import Once from "./Once.svelte"
    import ComponentEvents from "./ComponentEvents.svelte"
    import Outer from "./Nested/Outer.svelte"

    function handleMessage(event) {
		alert(event.detail.text);
	}
</script>

<MouseEx />
<Once />
<ComponentEvents />
<Outer on:message={handleMessage}/>
