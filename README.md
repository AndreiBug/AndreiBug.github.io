<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>My Personal Page</title>

    <style>
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            color: #333;
        }

        header {
            background-color: #222;
            color: white;
            text-align: center;
            padding: 50px 20px;
        }

        header h1 {
            font-size: 40px;
            margin-bottom: 10px;
        }

        header p {
            font-size: 18px;
            color: #ccc;
        }

        nav {
            background-color: #333;
            text-align: center;
            padding: 15px;
        }

        nav a {
            color: white;
            text-decoration: none;
            margin: 0 15px;
        }

        nav a:hover {
            color: #4caf50;
        }

        section {
            max-width: 900px;
            margin: 40px auto;
            padding: 30px;
            background-color: white;
            border-radius: 10px;
            box-shadow: 0 3px 10px rgba(0, 0, 0, 0.1);
        }

        section h2 {
            margin-bottom: 20px;
            color: #222;
        }

        .skills {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
        }

        .skill {
            background-color: #4caf50;
            color: white;
            padding: 10px 15px;
            border-radius: 20px;
        }

        footer {
            text-align: center;
            background-color: #222;
            color: white;
            padding: 20px;
            margin-top: 40px;
        }
    </style>
</head>

<body>

    <header>
        <h1>Andrei Costache</h1>
        <p>Student | Developer | Technology Enthusiast</p>
    </header>

    <nav>
        <a href="#about">About Me</a>
        <a href="#skills">Skills</a>
        <a href="#projects">Projects</a>
        <a href="#contact">Contact</a>
    </nav>

    <section id="about">
        <h2>About Me</h2>
        <p>
            Hello! My name is Andrei and I am a student interested in
            software development, computer networks and modern technologies.
            I enjoy learning new technologies and working on interesting
            projects.
        </p>
    </section>

    <section id="skills">
        <h2>Skills</h2>

        <div class="skills">
            <div class="skill">HTML</div>
            <div class="skill">CSS</div>
            <div class="skill">JavaScript</div>
            <div class="skill">Python</div>
            <div class="skill">Linux</div>
            <div class="skill">Git</div>
        </div>
    </section>

    <section id="projects">
        <h2>Projects</h2>

        <h3>Personal Project</h3>
        <p>
            A project developed as part of my university studies,
            focused on software development and automation.
        </p>

        <br>

        <h3>University Projects</h3>
        <p>
            Various projects involving programming, computer networks,
            web development and software engineering.
        </p>
    </section>

    <section id="contact">
        <h2>Contact</h2>

        <p>Email: your.email@example.com</p>
        <p>GitHub: github.com/your-username</p>
    </section>

    <footer>
        <p>&copy; 2026 Andrei Costache. All rights reserved.</p>
    </footer>

</body>

</html>
