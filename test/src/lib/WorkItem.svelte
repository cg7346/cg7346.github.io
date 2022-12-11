<script>
    export let id;
    export let position;
    export let company;
    export let location;
    export let startDate;
    export let endDate;
    export let subtitle;
    export let summary;
    export let results = [{title: '', description: ''}];
    export let publications = [{title: '', link: '', description: ''}];
</script>

<main>
    <section class="work-item" id="work-{id}">

        <input id="work-item-{id}" type="checkbox" class="toggle-item" checked hidden/>
        <label for="work-item-{id}" hidden></label>

        <header>
            <div class="position">{position}</div>
            <div class="company">{company}, {location}</div>
            <div class="date">
                <span class="endDate">{startDate} - {endDate}</span>
            </div>
        </header>
        {#if subtitle != ''}
            <span><em>{subtitle}</em></span>
        {/if}
        <div class="item">
            <div class="summary">
                <p>{summary}</p>
            </div>
            <div class="highlights">
                <strong>Results</strong>
                {#each results as { title, description }}
                    <li><em>{title}</em> - {description}</li>
                {/each}
  
                {#each publications as { title, link, description }, i}
                    {#if title != ''}
                        <li><em>{title}</em><a target="_blank" href={link}>{description}</a></li>
                    {/if}
                {/each}
            </div>
        </div>
    </section>
</main>