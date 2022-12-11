<script>
    export let name;
    export let jobTitle;
    export let phoneNumber;
    export let email;
    export let linkedIn;
    export let github;
</script>
  
<main>
    <header id="header" class="clear">
        <!-- The (first) h1 will be used as the <title> of the HTML page -->
        <div>
        <!-- TODO: convert to a name and major form variable -->
            <h1 class="name">{name}</h1>
            <h2 class="label">{jobTitle}</h2>
        </div>
        <!-- The unordered list immediately after the h1 will be formatted on a single
            line. It is intended to be used for contact details -->
        <div id="contactInfo">
            <!-- <div id="contact"> -->
            <div class="phone">
                <span class="fa fa-mobile"></span>
                <!--  TODO: convert into a phone number form variable  -->
                <a href="tel:{phoneNumber}">{phoneNumber}</a>
            </div>
            <div class="email">
                <span class="fa fa-envelope-o"></span>
                <!--  TODO: convert into a email form variable  -->
                <a href="mailto:{email}">{email}</a>
            </div>
            <!--                    </div>-->

            <!--                    <div id="profiles">-->
            <!--                    <div class="item">-->
            <div class="website">
                <span class="fa fa-linkedin-square"></span>
                    <!--  TODO: insert LinkedIn link form variable  -->
                <a target="_blank" href="http://www.linkedin.com/{linkedIn}">{linkedIn}</a>
            </div>
            <!--        </div>-->
            <!--        <div class="item">-->
            <div class="website">
                <span class="fa fa-github-square"></span>
                <!--  TODO: insert GitHub link form variable  -->
                <a target="_blank" href="https://{github}">{github}</a>
            </div>
            <!--                    </div>-->
        </div>
        <!--                </div>-->
    </header>
</main>
  