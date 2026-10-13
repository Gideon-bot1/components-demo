<script>
    //import Picture from "./card-internals/Picture.svelte";
    import Details from "./card-internals/Details.svelte";
    let { person } = $props()

    /*let person = 
    {
        fullName: "Phill Conners",
        favouriteSong: "I Got You Babe",
        petsName:"Punxsutawney"
    }
    */
</script>

<article class="card">
    <Picture image={person.image}/>
    <Details person = {person} />
</article>

<style>
    .card {
        display: flex;
        align-items: center;
        gap: 2rem;
        border: 1px solid #ccc;
        border-radius: 5px;
        padding: 1rem;
        max-width: 600px;
        margin: 1rem;
    }
</style>
