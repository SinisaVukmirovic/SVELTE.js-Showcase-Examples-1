<script>
    let adjective = '';
</script>

<style>
    p {
        font-size: 2.5rem;
        text-align: center;
        color: cornflowerblue;
    }
    strong {
        font-size: 4rem;
    }
</style>

<h3>Describe Svelte.js</h3>
<input type="text" placeholder="Describe Svelte" bind:value={adjective}>
<p>Svelte.js is - <strong>{adjective || 'amazing'}!</strong></p>