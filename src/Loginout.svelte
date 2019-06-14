<script>
    let user = { loggedIn: false };

    const toggleLog = () => {
        user.loggedIn = !user.loggedIn;
    }
</script>

{#if user.loggedIn}
    <button on:click={toggleLog}>
        Log Out
    </button>
{:else}
    <button on:click={toggleLog}>
        Log In
    </button>
{/if}