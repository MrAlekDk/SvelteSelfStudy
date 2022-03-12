<script>
import Nested from "./Nested/NestedObject.svelte"
const person ={
    name : 'Alexander',
    age : 23,
    city : 'Albertslund',
    education : 'Computer science'
}
</script>

<Nested {...person}/>

