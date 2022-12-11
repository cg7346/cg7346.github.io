<script>
    export let summary;
    export let keyCourses;
</script>
  
<main>
    <section class="section main-summary">
        <section>
            <!--  TODO: convert into a main summary form text box  -->
            <div class="main-summary">
                <p>{summary}</p>
            </div>
            <table class="center">
                <!--  TODO: enter number of columns and rows for table  -->
                <tr>
                    <td>
                        <ul>
                            <li>{keyCourses[0]}</li>
                            <li>{keyCourses[1]}</li>
                            <li>{keyCourses[2]}</li>
                        </ul>
                    </td>
                    <td>
                        <ul>
                            <li>{keyCourses[3]}</li>
                            <li>{keyCourses[4]}</li>
                            <li>{keyCourses[5]}</li>
                        </ul>
                    </td><!---->
                </tr>
            </table>
        </section>
    </section>
</main>
  