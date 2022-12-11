<script>
	import WorkItem from './lib/WorkItem.svelte';
    import { Card, CardBody } from 'sveltestrap';
    import Header from './lib/Header.svelte';
    import Objective from './lib/Objective.svelte';
    import Education from './lib/Education.svelte';
    import Publication from './lib/Publication.svelte';
    import Experience from './lib/Experience.svelte';

    const header = {
		name: 'CELESTE GAMBARDELLA',
        jobTitle: 'SOFTWARE ENGINEER',
        phoneNumber: '+1 (401) 603-8201',
        email: 'cg7346@rit.edu',
        linkedIn: 'in/celeste-gambardella',
        github: 'github.com/cg7346'
	};

    const objective = {
        summary: `An experienced Software Engineer in user-interface focused on front-end web
                development, back-end Java for cloud-based products. Well-developed soft skills and understanding of how software engineering
                fits into the larger operations of a business. Easily able to adapt while learning new skills and
                seeking an opportunity to grow as a Software Engineering in a fast-pace environment as a Full Stack Software Engineer. Available May of 2023.
                Extensive experience in:`,
        keyCourses: ["Engineering of Software Subsystems", "Developing System Applications", "Systems Analysis and Design", "Business Intelligence & Data Mining", "Client-Focused Product Development", "Human-Centered Requirements & Design"]
    };

    const education = {
        major: "Software Engineering",
        degree: "Bachelor of Science",
        institution: "Rochester Institute of Technology",
        state: "NY",
        gradDate: "May 2023",
        minor: "Management Information Systems & Communications - Minor"
    };

    const workOne = {
        id: 1,
        position: 'Full-Stack Innovation Engineer Intern',
        company: "Nike, Inc. European Headquaters",
        location: "Netherlands",
        startDate: "Sep 2021",
        endDate: "Aug 2022",
        subtitle: '',
        summary: `Working in a multi-disciplinary team on various innovative projects to drive benefits for Nike through the "connected store initiative". With a team of engineers, scrum masters and product owners to envision and deliver robust applications and services that bring Nike omni-channel solutions to the next level. Involved designing and building secure, highly scalable, and innovative services in a continuous delivery model.`,
        results: [{title: `Cross-Team Collaborations`, description: `Enabled new collaborations with other teams within the organization`},
                  {title:  `Market Research`, description: `Analysis of off the shelf solutions versus building capabilities in house based off of research done on 32 companies`},
                  {title: `Front-End Application`, description: `Collaboratively developed version one of React and iOS front-end prototyping for first step in the "connected store initiative" for a framework to test "feasibility" for early prototyping and testing`}],
        publications: [{title: '', link: '', description: ''}]
    };

    const workTwo = {
        id: 2,
        position: 'Security Software Engineer Intern',
        company: "U.S. Air Force Research",
        location: "NY",
        startDate: "May 2020",
        endDate: "August 2021",
        subtitle: 'Contractor: Rochester Institute of Technology]',
        summary: `Project lead and coordinator of the team’s efforts performing product launches and demos.
                            Designed and developed AI and Natural Language Processing (NLP) based cybersecurity analysis
                            tools to perform Cyber Vulnerability Assessments of System Requirements Specifications.
                            Analysis of algorithms results with incremental improvement, testing, and peer
                            validation.`,
        results: [{title: `Java Application`, description: `Developed algorithms using NLP and Alloy Modeling that
                            identifies security requirement defects, classifications, misuse cases, and attack
                            scenarios. 4.2% improvement of analyzed results.`},
                  {title:  `Product Demonstration`, description: `Assembled necessary security requirements that showcase
                            all features for the current application being used when presenting our findings to other
                            companies.`}],
        publications: [{title: `Published Paper: `, link: `https://ieeexplore.ieee.org/document/9582360/`, description: `A Natural Language Processing Technique for Formalization of Systems Requirement Specifications`}]
    };

    const workThree = {
        id: 3,
        position: 'Application Developer Intern',
        company: "Gabriel Software LLC",
        location: "MA",
        startDate: "Jun 2019",
        endDate: "Jan 2020",
        subtitle: '',
        summary: `Programmed modules and routines based on design specifications as prepared by the product
                            management team using the Azure Cloud Development System. Collaboratively developed customer
                            solutions and employed new technologies and coding strategies to create and maintain the
                            company’s state-of-the-art product. Implemented new features requested by customers.`,
        results: [{title: `New Application Features`, description: `Creation of text and email messaging feature using
                            Twilio’s API and an autofill search bar for members using JavaScript and HTML. Which helped
                            refine and design these features. Adaptively learned Twilio’s API and tested while debugging
                            from within SQL Server Management Studio, Visual Studio, and Chrome’s DevTools.`},
                  {title:  `Redesigned Reports`, description: `Conversion of Crystal Reports to SQL Server Reporting Services
                            (SSRS), a more customizable report, for their users in VB.NET. Collaborated with customer
                            feedback and desired results to restructure new reports that are easily generated for
                            customers.`}],
        publications: [{title: '', link: '', description: ''}]
    };

    const publicationOne = {
        id: 4,
        num: 1,
        link: `https://saunders.rit.edu/blog/2020/04/saunders-students-study-organizational-behavior-during-covid-19-pandemic`,
        title: `COVID-19 Organizational Behavior Study`,
        publisher: `Saunder College of Business`,
        date: 'April 2020',
        description: `Analyzed how the public was responding to the coronavirus with a Tweet Analysis. Used Twitter's API to collect tweets about COVID-19 from the World Health Organization (WHO). The analysis of the data collected was conducted in
                            Orange 3 that enhances data visualization, machine learning, and data mining. Through
                            Twitter’s API and Orange 3 I pin-pointed particular events trigger a set
                            of emotions among people. More often than not these were Surprise, Joy, and Anger.`
    };

    const experienceOne = {
        id: 1,
        title: `Software Engineer Freshman Seminar Course Assistant`,
        company: 'Rochester Institute of Technology',
        startDate: 'Aug 2019',
        endDate: 'Dec 2019',
        summary: `Worked cohesively with professors and students to enhance students' experience and creating a
                            productive learning environment.`
    };

    const experienceTwo = {
        id: 2,
        title: `Women’s Soccer (Club Captain)`,
        company: 'Rochester Institute of Technology',
        startDate: 'Aug 2018',
        endDate: 'Present',
        summary: `Integral leader on the team with an average of 7 goals a season, guiding the team to the
                            NIRSA Region 1 regionals for 4 years.`
    };
  </script>
  
  <main>
    <body>
        <div id="resume">
            <!--  CONTACT  -->
            <Header {...header}/>

            <!-- The paragraph after the h1 and ul and before the first h2 is optional. It 
                is intended to be used for a short summary. -->
            <!-- PROFILE -->
            <Objective {...objective}/>

            <!-- You have to wrap the "left" and "right" half of these headings in spans by
                hand -->
            <!--  EDUCATION  -->
            <Education {...education} />

            <!--      RELEVANT EXPERIENCE       -->
            <!--     You have to wrap the "left" and "right" half of these headings in spans by hand-->
            <section class="section">
                <header>
                    <h2 class='section-title'>RELEVANT EXPERIENCE</h2>
                </header>
                <section id="work">
                    <!-- EXPERIENCE 1 -->
                    <WorkItem {...workOne} />
                    <!-- EXPERIENCE 2 -->
                    <WorkItem {...workTwo} />
                    <!-- EXPERIENCE 3 -->
                    <WorkItem {...workThree} />
                    <!-- PUBLICATION -->
                    <Publication {...publicationOne} />
                </section>
            </section>

            <!--      EXPERIENCE      -->
            <section class="section">
                <header>
                    <h2 class='section-title'>EXPERIENCE</h2>
                </header>
                <section id="awards">
                    <!-- Item 1 -->
                    <Experience {...experienceOne} />
                    <!-- Item 2 -->
                    <Experience {...experienceTwo} />
                </section>
            </section>
        </div>
    </body>
  </main>
  