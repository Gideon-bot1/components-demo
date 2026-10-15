<script>
    import Header from "$lib/Components/Header.svelte";
    import Footer from "$lib/Components/Footer.svelte";

    let firstName = $state();
    let lastName = $state();
    let fullName = $derived(firstName + " " + lastName)

    firstName = "Web"
    lastName = "One"
</script>


    <h2>Header?</h2>

    {#if firstName && lastName}
    <p>Hi, {fullName}!</p>
    {/if}
