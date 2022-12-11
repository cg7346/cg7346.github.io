<script>
    export let major;
    export let degree;
    export let institution;
    export let state;
    export let gradDate;
    export let minor;
</script>

<main>
    <section class="section">
        <header>
            <h2 class='section-title'>EDUCATION <span class="item-count"></span></h2>
        </header>

        <section id="education">
            <section class="education-item">
                <header>
                    <div class="area">{major},</div>
                    <div class="studyType">{degree}</div>
                    <div class="institution">{institution}, {state}</div>
                    <div class="date">
                        <span class="endDate">{gradDate}</span>
                    </div>
                    <span class="minor">
                    <br><em>{minor}</em>
                </span>
                </header>

            </section>
        </section>
    </section>
</main>