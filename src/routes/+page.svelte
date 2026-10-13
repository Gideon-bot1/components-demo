<script>
    import Card from '$lib/components/Card.svelte';
    import Luke from '$lib/assets/images/Lukeimg.jpg'
    let people = [
            {
            fullName: "Phill Conners",
            favouriteSong: "I Got You Babe",
            petsName:"Punxsutawney",
            image: "https://discover.hubpages.com/.image/MTc0NDQ4NDQ5OTAxNTY5Njcw/the-benefits-of-strongman.jpg?profile=w828&x=50&y=50",
        },
            {
            fullName: "Rhichie Rich",
            favouriteSong: "I Got You Babe",
            petsName:"Slimer",
            image: "",
        },
            {
            fullName: "Luke Uke",
            favouriteSong: "I Got You Babe",
            petsName:"Big Dawg",
            image: "src/lib/assets/images/Lukeimg.jpg",
        },
                    {
            fullName: "Luke Uke",
            favouriteSong: "I Got You Babe",
            petsName:"Boss Man",
            image: "",
        },
    ];
</script>

<main>
<!--TODO make this a loop-->
{#each people as person}
    <Card person = {person}/>
{/each}
</main>

<style>
    main {
        display: flex;
        flex-wrap: wrap;
    }
</style>