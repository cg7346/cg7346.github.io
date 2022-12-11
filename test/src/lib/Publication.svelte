<script>
    export let id;
    export let num;
    export let link;
    export let title;
    export let publisher;
    export let date;
    export let description;
</script>

<main>
    <section class="publication-item" id="work-{id}">
        <input id="publication-item-{num}" type="checkbox" class="toggle-item" checked hidden/>
        <label for="publication-item-{num}" hidden></label>
        <header>
            <span class="name">
               <a target="_blank" href={link}>{title}</a>
            </span>
            <span class="publisher">in {publisher}</span>
            <div class="date">
                <span class="endDate">{date}</span>
            </div>
        </header>

        <div class="item">
            <div class="summary">
                <p><em>Publication</em> - {description}</p>
            </div>
        </div>
    </section>
</main>