<script>
import Person from "./Person.svelte"

    let people = [
        {id:1, name:"Alexander"},
        {id:2, name:"Anders"},
        {id:3, name:"Peter"},
        {id:4, name:"Carsten"}
    ];

    function removePerson(){
        people = people.splice(1);
    }
</script>

<button on:click={removePerson}>Remove first person</button>

{#each people as person (person.id)}
<Person name ={person.name}/>
{/each}