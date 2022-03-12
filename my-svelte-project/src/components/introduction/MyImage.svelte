<script>
	let src = "./images/jsbackground.png";
    export let altObject;
</script>

<img src = {src} alt = "A image of a {altObject}" class="myImg">
<p>Look at my styling, it's only located in the "MyImage.svelte" file and will only affect me</p>

<style>
    .myImg{
        height: 300px;
    }

    p {
        color:purple;
        font-weight: bolder;
    }
</style>