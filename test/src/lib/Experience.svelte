<script>
    export let id;
    export let title;
    export let company;
    export let startDate;
    export let endDate;
    export let summary;
</script>

<main>
    <section class="award-item">
        <input id="award-item-{id}" type="checkbox" class="toggle-item" checked hidden/>
        <label for="award-item-{id}" hidden></label>

        <header>
            <div class="title">
                {title}
            </div>
            <div class="awarder">
                {company}
            </div>
            <div class="date">
                <span class="endDate">{startDate} - {endDate}</span>
            </div>
        </header>

        <div class="item">
            <div class="summary">
                <p>{summary}</p>
            </div>
        </div>
    </section>
</main>