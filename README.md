<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Andrei-Darius Costache | Portfolio</title>

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            scroll-behavior: smooth;
        }

        :root {
            --background: #f4f6f8;
            --card: #ffffff;
            --text: #222222;
            --secondary: #666666;
            --primary: #2563eb;
            --primary-hover: #1d4ed8;
            --border: #e5e7eb;
            --nav: rgba(255, 255, 255, 0.9);
        }

        body.dark {
            --background: #111827;
            --card: #1f2937;
            --text: #f9fafb;
            --secondary: #d1d5db;
            --primary: #60a5fa;
            --primary-hover: #93c5fd;
            --border: #374151;
            --nav: rgba(17, 24, 39, 0.9);
        }

        body {
            font-family: Arial, sans-serif;
            background-color: var(--background);
            color: var(--text);
            line-height: 1.6;
            transition: background-color 0.3s, color 0.3s;
        }

        /* NAVBAR */

        nav {
            position: sticky;
            top: 0;
            z-index: 100;
            background-color: var(--nav);
            backdrop-filter: blur(10px);
            border-bottom: 1px solid var(--border);
            padding: 15px 30px;

            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        nav .logo {
            font-size: 20px;
            font-weight: bold;
        }

        nav .links {
            display: flex;
            align-items: center;
            gap: 25px;
        }

        nav a {
            color: var(--text);
            text-decoration: none;
            font-size: 15px;
        }

        nav a:hover {
            color: var(--primary);
        }

        #themeButton {
            border: none;
            background: var(--text);
            color: var(--background);
            padding: 8px 14px;
            border-radius: 20px;
            cursor: pointer;
            font-size: 14px;
        }

        #themeButton:hover {
            opacity: 0.8;
        }

        /* HERO */

        .hero {
            min-height: 85vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            padding: 40px 20px;
        }

        .hero h1 {
            font-size: 55px;
            margin-bottom: 10px;
        }

        .hero h2 {
            font-size: 25px;
            color: var(--primary);
            margin-bottom: 20px;
        }

        .hero p {
            max-width: 650px;
            color: var(--secondary);
            font-size: 18px;
        }

        .buttons {
            margin-top: 30px;
            display: flex;
            gap: 15px;
        }

        .button {
            text-decoration: none;
            padding: 12px 22px;
            border-radius: 8px;
            background-color: var(--primary);
            color: white;
            font-weight: bold;
            transition: 0.2s;
        }

        .button:hover {
            background-color: var(--primary-hover);
            transform: translateY(-2px);
        }

        .button.secondary {
            background-color: transparent;
            color: var(--text);
            border: 1px solid var(--border);
        }
        
        .profile-picture {
            width: 180px;
            height: 180px;
            object-fit: cover;
            border-radius: 50%;
            border: 4px solid var(--primary);
            margin-bottom: 25px;
            box-shadow: 0 8px 25px rgba(0, 0, 0, 0.2);
            transition: transform 0.3s ease;
        }

        .profile-picture:hover {
            transform: scale(1.05);
        }

        /* SECTIONS */

        section {
            max-width: 1000px;
            margin: 0 auto;
            padding: 80px 25px;
        }

        section h2 {
            font-size: 32px;
            margin-bottom: 30px;
            border-bottom: 2px solid var(--primary);
            padding-bottom: 10px;
        }

        .card {
            background-color: var(--card);
            border: 1px solid var(--border);
            border-radius: 12px;
            padding: 25px;
            margin-bottom: 20px;
            transition: 0.3s;
        }

        .card:hover {
            transform: translateY(-3px);
        }

        .card h3 {
            margin-bottom: 5px;
        }

        .date {
            color: var(--primary);
            font-size: 14px;
            font-weight: bold;
        }

        .card p {
            color: var(--secondary);
            margin-top: 10px;
        }

        /* SKILLS */

        .skills {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
        }

        .skill {
            background-color: var(--card);
            border: 1px solid var(--border);
            padding: 10px 15px;
            border-radius: 20px;
            transition: 0.2s;
        }

        .skill:hover {
            border-color: var(--primary);
            color: var(--primary);
        }

        /* PROJECT LINKS */

        .project-link {
            display: inline-block;
            margin-top: 15px;
            color: var(--primary);
            text-decoration: none;
            font-weight: bold;
        }

        .project-link:hover {
            text-decoration: underline;
        }

        /* CONTACT */

        .contact {
            text-align: center;
        }

        .contact a {
            color: var(--primary);
            text-decoration: none;
        }

        /* FOOTER */

        footer {
            text-align: center;
            padding: 30px;
            border-top: 1px solid var(--border);
            color: var(--secondary);
        }

        /* MOBILE */

        @media (max-width: 700px) {

            nav .links a {
                display: none;
            }

            .hero h1 {
                font-size: 38px;
            }

            .hero h2 {
                font-size: 20px;
            }

            section {
                padding: 60px 20px;
            }
        }
    </style>
</head>

<body>

    <!-- ================= NAVBAR ================= -->

    <nav>

        <div class="links">
            <a href="#about">About</a>
            <a href="#experience">Experience</a>
            <a href="#projects">Projects</a>
            <a href="#education">Education</a>
            <a href="#skills">Skills</a>
            <a href="#contact">Contact</a>

            <button id="themeButton" onclick="toggleTheme()">
                🌙 Dark
            </button>
        </div>

    </nav>


    <!-- ================= HERO ================= -->

    <div class="hero">
    
        <img src="profile.jpg" 
         alt="Andrei-Darius Costache" 
         class="profile-picture">
         
        <h1>Andrei-Darius Costache</h1>

        <h2>Junior QA Engineer & Computer Science Student</h2>

        <p>
            I'm a Computer Science student passionate about software testing,
            networking, programming and modern technologies. I enjoy building
            projects and learning how complex systems work.
        </p>

        <div class="buttons">

            <a class="button"
               href="https://github.com/AndreiBug"
               target="_blank">
                GitHub
            </a>

            <a class="button secondary"
               href="https://www.linkedin.com/in/andrei-darius-costache-043a9923a"
               target="_blank">
                LinkedIn
            </a>

        </div>

    </div>


    <!-- ================= ABOUT ================= -->

    <section id="about">

        <h2>About Me</h2>

        <div class="card">

            <p>
                I am a Computer Science student at the National University
                of Science and Technology Politehnica Bucharest. My main
                interests include software quality assurance, computer
                networks, programming and cybersecurity.
            </p>

            <p>
                Currently, I work as a Junior QA Engineer, where I perform
                manual testing and collaborate with development teams to
                ensure software quality.
            </p>

        </div>

    </section>


    <!-- ================= EXPERIENCE ================= -->

    <section id="experience">

        <h2>Work Experience</h2>

        <div class="card">

            <span class="date">Apr. 2026 - Present</span>

            <h3>Junior QA Engineer — Systematic</h3>

            <p>
                Perform manual testing on software applications, including
                functional, regression, smoke and exploratory testing.
                Identify and report defects and collaborate with development
                teams to improve product quality.
            </p>

        </div>


        <div class="card">

            <span class="date">July 2025 - Oct. 2025</span>

            <h3>Networking Intern — Poșta Română</h3>

            <p>
                Assisted in configuring and maintaining network infrastructure
                across multiple branches. Worked with IP addressing, VLANs
                and routing protocols while helping improve LAN/WAN performance
                and reliability.
            </p>

        </div>

    </section>


    <!-- ================= PROJECTS ================= -->

    <section id="projects">

        <h2>Projects</h2>


        <div class="card">

            <span class="date">June 2025 - Sept. 2025</span>

            <h3>Photovoltaic Community Simulation</h3>

            <p>
                Developed a Python-based simulation of a residential energy
                community with a shared photovoltaic system. Implemented
                data preprocessing, photovoltaic sizing optimization using
                Differential Evolution and a multi-agent recommendation
                system.
            </p>

            <a class="project-link"
               href="https://github.com/AndreiBug/Photovoltaic-Community-Simulation"
               target="_blank">
                View on GitHub →
            </a>

        </div>


        <div class="card">

            <span class="date">Jan. 2025</span>

            <h3>Diabetes Prediction</h3>

            <p>
                Developed a machine learning model in Python for diabetes
                prediction using PCA and supervised classifiers such as
                SVM and KNN. Worked with preprocessing, normalization,
                dimensionality reduction and model evaluation.
            </p>

            <a class="project-link"
               href="https://github.com/AndreiBug/Diabetes-Prediction"
               target="_blank">
                View on GitHub →
            </a>

        </div>


        <div class="card">

            <span class="date">July 2024 - Sept. 2024</span>

            <h3>Finding The Milk</h3>

            <p>
                Created a 2D wave-based shooter game using Unity and C#.
                Implemented health, reload, damage and wave systems,
                together with gameplay mechanics and cutscenes.
            </p>

            <a class="project-link"
               href="https://github.com/AndreiBug/Finding-The-Milk"
               target="_blank">
                View on GitHub →
            </a>

        </div>


        <div class="card">

            <span class="date">Mar. 2023 - May 2023</span>

            <h3>Tournament Simulation</h3>

            <p>
                Developed a LAN tournament simulation in C using linked lists,
                stacks, queues and binary trees. Automated program execution
                and validation using Bash scripts.
            </p>

            <a class="project-link"
               href="https://github.com/AndreiBug/Tournament-Simulation"
               target="_blank">
                View on GitHub →
            </a>

        </div>

    </section>


    <!-- ================= EDUCATION ================= -->

    <section id="education">

        <h2>Education</h2>

        <div class="card">

            <span class="date">Oct. 2026 - June 2028</span>

            <h3>
                National University of Science and Technology
                Politehnica Bucharest
            </h3>

            <p>
                Master's Degree — Faculty of Automatic Control and
                Computer Science
            </p>

        </div>


        <div class="card">

            <span class="date">Sept. 2022 - June 2026</span>

            <h3>
                National University of Science and Technology
                Politehnica Bucharest
            </h3>

            <p>
                Bachelor's Degree — Faculty of Automatic Control and
                Computer Science
            </p>

        </div>

    </section>


    <!-- ================= CERTIFICATIONS ================= -->

    <section id="certifications">

        <h2>Certifications & Courses</h2>

        <div class="card">

            <h3>Cisco Networking Academy — CCNA 1, 2 & 3</h3>

            <p>
                Network fundamentals, VLANs, routing protocols, subnetting,
                wireless networking, ACLs, VPNs and practical Cisco Packet
                Tracer labs.
            </p>

        </div>


        <div class="card">

            <h3>CompTIA Security+</h3>

            <p>
                Cybersecurity fundamentals covering network security,
                risk management, cryptography, threat analysis and
                incident response.
            </p>

        </div>

    </section>


    <!-- ================= SKILLS ================= -->

    <section id="skills">

        <h2>Skills</h2>

        <div class="skills">

            <div class="skill">C</div>
            <div class="skill">C++</div>
            <div class="skill">C#</div>
            <div class="skill">Python</div>
            <div class="skill">Java</div>
            <div class="skill">JavaScript</div>
            <div class="skill">HTML</div>
            <div class="skill">CSS</div>
            <div class="skill">SQL</div>
            <div class="skill">MATLAB</div>
            <div class="skill">Spring Boot</div>
            <div class="skill">Linux</div>
            <div class="skill">Git</div>
            <div class="skill">Networking</div>
            <div class="skill">OOP</div>
            <div class="skill">Manual Testing</div>
            <div class="skill">QA</div>
        </div>

    </section>


    <!-- ================= CONTACT ================= -->

    <section id="contact" class="contact">

        <h2>Contact</h2>

        <div class="card">

            <p>
                <strong>Email:</strong>
                <a href="mailto:costache.andrei.darius@gmail.com">
                    costache.andrei.darius@gmail.com
                </a>
            </p>

            <p>
                <strong>GitHub:</strong>
                <a href="https://github.com/AndreiBug" target="_blank">
                    github.com/AndreiBug
                </a>
            </p>

            <p>
                <strong>LinkedIn:</strong>
                <a href="https://www.linkedin.com/in/andrei-darius-costache-043a9923a"
                   target="_blank">
                    LinkedIn Profile
                </a>
            </p>

        </div>

    </section>


    <!-- ================= FOOTER ================= -->

    <footer>

        <p>
            © 2026 Andrei-Darius Costache
        </p>

    </footer>


    <!-- ================= DARK MODE ================= -->

    <script>

        function toggleTheme() {

            document.body.classList.toggle("dark");

            const button = document.getElementById("themeButton");

            if (document.body.classList.contains("dark")) {
                button.innerHTML = "☀️ Light";
            } else {
                button.innerHTML = "🌙 Dark";
            }
        }

    </script>

</body>
</html>
