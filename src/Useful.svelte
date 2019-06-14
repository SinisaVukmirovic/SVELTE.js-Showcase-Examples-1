<script>
    let usefulLinks = [
        {
            id: 'Quote-Generator-about-Scholes/',
            name: 'Quotes About Paul Scholes'
        },
        {
            id: 'Are-You-Being-Watched-Right-Now/',
            name: 'Are You Being Watched Right Now?'
        },
        {
            id: 'Movie-Info-Search-App/',
            name: 'Search for Movies by Title'
        },
        {
            id: 'Web-Devs-Tracker/',
            name: 'YT Web Developers Tracker'
        },
        {
            id: 'Stopwatch-Timer/',
            name: 'Need a Timer?'
        },
        {
            id: 'GIF-Search-App/',
            name: 'Searcn For GIFs'
        }
    ];
</script>

<style>
    ul {
        list-style: none;
    }
    li {
        margin: .5em;
    }
</style>

<h3>Useful Links:</h3>

<ul>
    {#each usefulLinks as { id, name }, i}
        <li><a target="_blank" href="https://sinisavukmirovic.github.io/{id}">
            {i + 1}. {name}
        </a></li>
    {/each}
</ul>