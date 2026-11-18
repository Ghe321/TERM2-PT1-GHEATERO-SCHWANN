<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Ghea Lorraine | My Portfolio</title>

<link href="https://fonts.googleapis.com/css2?family=Arial&family=Nunito:wght@400;500;600;700&family=Courier+Prime&display=swap" rel="stylesheet">

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    scroll-behavior: smooth;
}

body {
    background-color: #f4f3e9;
    color: #344638;
    font-family: 'Nunito', sans-serif;
    font-size: 14px;
}

.navbar {
    background-color: #354c39;
    color: white;
    padding: 18px 7%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    gap: 15px;
}

.logo {
    font-family: 'Courier Prime', monospace;
    font-size: 19px;
    font-weight: bold;
}

.logo span {
    color: #b8c9a9;
}

.nav-links {
    list-style: none;
    display: flex;
    gap: 17px;
    flex-wrap: wrap;
}

.nav-links a {
    color: white;
    text-decoration: none;
    font-size: 12px;
}

.nav-links a:hover {
    color: #b8c9a9;
}

.container {
    width: 86%;
    max-width: 1000px;
    margin: auto;
}

.hero {
    margin-top: 30px;
    padding: 45px 35px;
    background-color: #dfe7d6;
    border: 1px solid #c5d0bc;
}

.small-label {
    font-family: 'Courier Prime', monospace;
    font-size: 11px;
    letter-spacing: 1px;
    margin-bottom: 18px;
    color: #52684e;
}

.hero h1 {
    font-family: 'Nunito', sans-serif;
    font-size: clamp(35px, 6vw, 56px);
    line-height: 1.2;
    color: #304936;
}

.hero h1 span {
    display: block;
    color: #718766;
}

.hero p {
    max-width: 480px;
    line-height: 1.9;
    margin-top: 15px;
    color: #586656;
}

.hero-label {
    display: inline-block;
    margin-top: 20px;
    padding: 8px 12px;
    border: 1px solid #aebda4;
    font-size: 11px;
}

.section {
    margin-top: 45px;
    scroll-margin-top: 25px;
}

.section-heading {
    display: flex;
    align-items: center;
    gap: 12px;
    margin-bottom: 20px;
}

.section-number {
    font-family: 'Courier Prime', monospace;
    color: #738668;
    border: 1px solid #c4d0b9;
    padding: 7px 9px;
}

.section-heading h2 {
    font-size: 25px;
    font-weight: 700;
    color: #344b37;
}

.section-subtitle {
    font-size: 12px;
    color: #7a8173;
    margin-top: 2px;
}

/* ABOUT */

.about-card {
    background-color: #fffef8;
    border: 1px solid #d8ddcf;
    padding: 25px;
    display: grid;
    grid-template-columns: 1fr 170px;
    gap: 25px;
    align-items: center;
}

.about-card p {
    line-height: 2;
    color: #536052;
}

.about-note {
    background-color: #e8ecdf;
    padding: 20px 14px;
    text-align: center;
    border: 1px solid #d5ddca;
}

.about-note h3 {
    font-family: 'Courier Prime', monospace;
    font-size: 19px;
    color: #506749;
}

.about-note p {
    font-size: 12px;
    margin-top: 8px;
    line-height: 1.7;
}

/* HOBBIES */

.hobby-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 15px;
}

.hobby-card {
    background-color: #fffef8;
    border: 1px solid #d8ddcf;
    padding: 22px 18px;
}

.hobby-number {
    font-family: 'Courier Prime', monospace;
    font-size: 11px;
    color: #859478;
    margin-bottom: 18px;
}

.hobby-card h3 {
    font-size: 20px;
    margin-bottom: 10px;
    color: #405740;
}

.hobby-card p {
    font-size: 13px;
    line-height: 1.9;
    color: #657061;
}

/* SKILLS */

.skills-area {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
}

.skill {
    background-color: #e3e9dc;
    border: 1px solid #cbd5c2;
    color: #435a40;
    padding: 11px 15px;
    font-size: 13px;
}

/* PROJECT */

.project-card {
    background-color: #e2e8da;
    border: 1px solid #cbd5c2;
    padding: 28px;
}

.project-label {
    font-family: 'Courier Prime', monospace;
    font-size: 11px;
    letter-spacing: 1px;
    color: #667c5d;
    margin-bottom: 12px;
}

.project-card h3 {
    font-size: 25px;
    margin-bottom: 12px;
    color: #344b37;
}

.project-card p {
    max-width: 700px;
    font-size: 13px;
    line-height: 2;
    color: #536052;
    margin-bottom: 14px;
}

.project-tag {
    display: inline-block;
    border: 1px solid #b6c5aa;
    padding: 7px 10px;
    font-size: 11px;
    color: #4d6748;
}

/* DREAMS */

.dream-card {
    background-color: #fffef8;
    padding: 28px;
    border: 1px solid #d8ddcf;
}

.dream-card h3 {
    font-size: 25px;
    color: #405740;
    margin-bottom: 15px;
}

.dream-card p {
    font-size: 13px;
    line-height: 2;
    color: #586656;
}

.dream-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 8px;
    margin-top: 18px;
}

.dream-tags span {
    background-color: #e8ecdf;
    padding: 8px 11px;
    font-size: 11px;
    color: #4e6548;
    border: 1px solid #d5ddca;
}

/* QUOTE */

.quote {
    text-align: center;
    padding: 30px 15px;
    margin-top: 40px;
    border-top: 1px solid #d4dacb;
    border-bottom: 1px solid #d4dacb;
}

.quote p {
    font-family: 'Courier Prime', monospace;
    font-size: 17px;
    color: #586e50;
}

.quote span {
    display: block;
    margin-top: 10px;
    font-size: 10px;
    letter-spacing: 1px;
    color: #777e70;
}

/* FOOTER */

footer {
    margin-top: 45px;
    padding: 25px 15px;
    text-align: center;
    background-color: #354c39;
    color: #e7ecdf;
    font-size: 12px;
    line-height: 1.9;
}

footer strong {
    font-family: 'Courier Prime', monospace;
    color: #c8d7bb;
}

/* MOBILE */

@media (max-width: 700px) {
    .navbar {
        flex-direction: column;
        align-items: flex-start;
        padding: 17px 5%;
    }

    .nav-links {
        gap: 12px;
    }

    .nav-links a {
        font-size: 11px;
    }

    .container {
        width: 92%;
    }

    .hero {
        padding: 30px 23px;
    }

    .hero h1 {
        font-size: 39px;
    }

    .about-card {
        grid-template-columns: 1fr;
        padding: 20px;
    }

    .hobby-grid {
        grid-template-columns: 1fr;
    }

    .section-heading h2 {
        font-size: 22px;
    }

    .project-card,
    .dream-card {
        padding: 22px;
    }
}
</style>
</head>

<body>

<nav class="navbar">
    <div class="logo">ghea's portfolio<span>.</span></div>

    <ul class="nav-links">
        <li><a href="#home">Home</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#hobbies">Hobbies</a></li>
        <li><a href="#skills">Skills</a></li>
        <li><a href="#projects">Projects</a></li>
        <li><a href="#dreams">Dreams</a></li>
    </ul>
</nav>

<main class="container">

    <section class="hero" id="home">
        <div class="small-label">PERSONAL PORTFOLIO / 2026</div>

        <h1>
            Ghea Lorraine
            <span>B. Tero</span>
        </h1>

        <p>
            A little dreamer with a love for stories,
            creativity, and the world around her.
            Growing at her own pace, one little step
            at a time.
        </p>

        <div class="hero-label">
            STUDENT | DREAMER | FUTURE PROFESSIONAL
        </div>
    </section>

    <section class="section" id="about">
        <div class="section-heading">
            <span class="section-number">01</span>
            <div>
                <h2>A Little About Me</h2>
                <div class="section-subtitle">The girl behind the pages</div>
            </div>
        </div>

        <div class="about-card">
            <p>
                Hi! I'm Ghea Lorraine B. Tero, a 13-year-old
                student at Jacinto P. Elpa National High School.
                My birthday is on August 16. I love writing,
                even if I can sometimes be as lazy as a sloth,
                and I never say no to good food. I'm still
                discovering who I want to become, but I'm
                interested in two paths: medicine and journalism.
                Whether I end up helping people through healthcare
                or sharing stories and important information,
                I hope to make a difference in my own way.
            </p>

            <div class="about-note">
                <h3>In bloom</h3>
                <p>
                    Learning, growing, and figuring things
                    out one day at a time.
                </p>
            </div>
        </div>
    </section>

    <section class="section" id="hobbies">
        <div class="section-heading">
            <span class="section-number">02</span>
            <div>
                <h2>Things I Love</h2>
                <div class="section-subtitle">Little joys in my everyday life</div>
            </div>
        </div>

        <div class="hobby-grid">
            <article class="hobby-card">
                <div class="hobby-number">HOBBY 01</div>
                <h3>Reading</h3>
                <p>
                    Getting lost in different worlds, discovering
                    new ideas, and finding stories that stay
                    with me long after the last page.
                </p>
            </article>

            <article class="hobby-card">
                <div class="hobby-number">HOBBY 02</div>
                <h3>Drawing</h3>
                <p>
                    Turning thoughts and imagination into
                    something visible, one line and one
                    little detail at a time.
                </p>
            </article>

            <article class="hobby-card">
                <div class="hobby-number">HOBBY 03</div>
                <h3>Watching Shows</h3>
                <p>
                    Enjoying different stories, interesting
                    characters, and the emotions that make
                    every show memorable.
                </p>
            </article>
        </div>
    </section>

    <section class="section" id="skills">
        <div class="section-heading">
            <span class="section-number">03</span>
            <div>
                <h2>Things I'm Good At</h2>
                <div class="section-subtitle">Skills I have and continue to develop</div>
            </div>
        </div>

        <div class="skills-area">
            <div class="skill">Creative Writing</div>
            <div class="skill">Creativity</div>
            <div class="skill">Observation</div>
        </div>
    </section>

    <section class="section" id="projects">
        <div class="section-heading">
            <span class="section-number">04</span>
            <div>
                <h2>My Projects</h2>
                <div class="section-subtitle">Little things I've worked on</div>
            </div>
        </div>

        <article class="project-card">
            <div class="project-label">PROJECT 01 / SCIENCE</div>

            <h3>Science Research</h3>

            <p>
                My research project gives me an opportunity to
                explore scientific questions, learn how to
                investigate a topic, and understand how research
                can help us discover useful information.
            </p>

            <span class="project-tag">Research and Investigation</span>
        </article>
    </section>

    <section class="section" id="dreams">
        <div class="section-heading">
            <span class="section-number">05</span>
            <div>
                <h2>Where I Hope to Go</h2>
                <div class="section-subtitle">A future I'm growing toward</div>
            </div>
        </div>

        <div class="dream-card">
            <h3>A life that makes a difference.</h3>

            <p>
                My dream is to become either a doctor or a
                journalist, build a successful life, and be
                financially comfortable. More than that, I want
                to become someone others can depend on in the
                future. I hope to help people who are poor,
                sick, or injured, and to share meaningful
                information that helps others understand the
                world around them. Whatever path I choose,
                I want my success to mean something beyond myself.
            </p>

            <div class="dream-tags">
                <span>Medicine</span>
                <span>Journalism</span>
                <span>Helping Others</span>
                <span>Personal Growth</span>
            </div>
        </div>
    </section>

    <div class="quote">
        <p>"Even the tallest trees began as something small."</p>
        <span>A NOTE TO MY FUTURE SELF</span>
    </div>

</main>

<footer>
    <strong>Ghea Lorraine B. Tero</strong><br>
    Growing through every season of life.
</footer>

</body>
</html>
