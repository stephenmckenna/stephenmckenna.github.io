<template>
    <div class='aboutMePage column items-center'>
        <p class="text-h4">About Me</p>
        <br/><br/>
        <div style='width: 1000px;' class='row items-center justify-between'>
            <img class='rounded-borders' style='height: 300px; width: auto;' src='./assets/photo.jpg' alt=''/>
            <p style='width: 750px;' class="text-body1 text-center">
            Hello! My name is Stephen McKenna, a senior Computer Science student at the University of Pittsburgh. Though most of my professional experience is in front-end engineering, in the future I hope to obtain a full-stack repertoire. This website is for me to present the work I have accomplished thus far in my career in technology. Here you'll find information about my education and past job experience, as well as a list of numerous projects I have completed both academically and recreationally.
            </p>
        </div>
        <br/><br/>
        <div style='width: 1000px;' class='row items-center justify-between q-mb-lg'>
            <p style='max-width: 500px;' class='text-body1 text-center'>
            I built this website from scratch in Visual Studio Code using VueJS and the Quasar Framework. Check out the source code on my
                <a class="bodyLinks" href='https://github.com/stephenmckenna' target='_blank' style='color: bg-accent; text-decoration: none;'><strong>GitHub</strong></a>!
            </p>
            <img class='rounded-borders' style='height: 300px; width: auto;' src='./assets/meAndCaia.jpeg' alt='' />
        </div>
        <q-parallax class='q-my-lg' scroll-target="body" speed='1' style='width: 1250px; height: 300px;' src='~assets/cathy.jpeg'>
            <div style='backdrop-filter: brightness(0.5); height: 100%; width: 100%'>
                <h2 class='text-white absolute-bottom-left' style='margin-left: 20px; bottom: -30px; text-decoration: underline'>UNIVERSITY OF PITTSBURGH</h2>
            </div>
        </q-parallax>
        <ul class='text-body1 q-my-lg'>
            <li>Expected graduation 12/2022</li>
            <li><strong>B.S. in Computer Science</strong>
                <ul>
                    <li><strong>Secondary field of study in Mathematics and Statistics</strong></li>
                </ul>
            </li>
            <li>Participating in Computer Science Club and Intramural Volleyball</li>
        </ul>
        <p class='text-body1 q-my-lg'>Current GPA: <strong>3.5</strong></p>
        <q-list class='column q-mt-lg' style='height:fit-content; max-height: 300px; width: 1250px;'>
            <q-item-label overline>Relevant Courses</q-item-label>
            <q-item-label caption>* - In progress</q-item-label>
            <q-item>
                <q-item-section>CS0401 - Intermediate Programming In Java</q-item-section>
            </q-item>
            <q-item>
                <q-item-section>CS0441 - Discrete Structures</q-item-section>
            </q-item>
            <q-item>
                <q-item-section>CS0445 - Data Structures</q-item-section>
            </q-item>
            <q-item>
                <q-item-section>CS0447 - Computer Organization and Assembly Language</q-item-section>
            </q-item>
            <q-item>
                <q-item-section>CS0449 - Introduction to Systems Software</q-item-section>
            </q-item>
            <q-item>
                <q-item-section>CS1501 - Algorithm Implementation</q-item-section>
            </q-item>
            <q-item>
                <q-item-section>CS1502 - Formal Methods in Computer Science</q-item-section>
            </q-item>
            <q-item>
                <q-item-section>CS1520 - Programming Languages for Web Applications</q-item-section>
            </q-item>
            <q-item>
                <q-item-section>CS1530 - Software Engineering</q-item-section>
            </q-item>
            <q-item>
                <q-item-section>CS1550 - Operating Systems</q-item-section>
            </q-item>
            <q-item>
                <q-item-section>CS1555 - Database Management Systems</q-item-section>
            </q-item>
            <q-item>
                <q-item-section>CS1566 - Introduction to Computer Graphics*</q-item-section>
            </q-item>
            <q-item>
                <q-item-section>CS1656 - Introduction to Data Science</q-item-section>
            </q-item>
        </q-list>
        <div style='height: 200px;'/>
    </div>
</template>

<script>


</script>