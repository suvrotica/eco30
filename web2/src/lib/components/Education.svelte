<script>
    export let phone_icon_image;
    export let education_list;
</script>
    
{#each education_list as level}
    <details>
        <summary>{level.stage} - {level.name}</summary>
        <nav>
            <ul>
                <li>{level.address}</li>
                <li><img src={phone_icon_image} alt="phone" />{level.phone}</li>
            </ul>
            <ul>
                <li>
                    <span><a role="button" href={level.href}>URL</a></span>
                </li>
            </ul>
        </nav>
        <p>{level.marks}<b>{level.years}</b></p>
    </details>
{/each}

<style>
    summary {
        font-weight: 200;
    }
    li,
    p,
    a {
        font-weight: 200;
        font-size: medium;
    }
</style>
