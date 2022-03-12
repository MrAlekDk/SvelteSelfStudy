<script>
   const colors = ['Blue','Red','Green','Yellow']
</script>

<h1>Great Colors</h1>

<ul>
    {#each colors as color}
    <li>{color}</li>
    {/each}
</ul>


<style>
    li{
        list-style: none;
    }
</style>