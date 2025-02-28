<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Portfolio</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            font-size: 16px;
            margin: 0;
            padding: 0;
            text-align: center;
            background-color: #d1c58c;
        }
        header {
            background: #333;
            color: white;
            padding: 20px;
        }
        section {
            padding: 20px;
        }
        .project {
            margin: 20px;
            padding: 10px;
            border: 2px solid #ddd;
        }
        button {
            padding: 10px 20px;
            background: #333;
            color: white;
            border: none;
            cursor: pointer;
        }
        h2{
            text-decoration: underline;
        }
    </style>
</head>
<body>
    <header>
        <h1>My Portfolio</h1>
    </header>
   
    <section>
        <h2>About Me</h2>
        <p>I am a B.Tech student in Electrical and Instrumentation Engineering with a strong ability to learn quickly and adapt to new environments. I excel at acquiring and applying knowledge effectively, making me skilled in problem-solving and innovation. Passionate about continuous learning, I thrive in dynamic settings and embrace new challenges. My goal is to bridge technology and engineering, contributing to innovative solutions. I am driven by curiosity, adaptability, and a commitment to professional growth in the ever-evolving tech industry.
 .</p>
    </section>
    <section>
        <h2>Achievements</h2>
        <div id="projects"></div>
    </section>
   <section>
    <h2> My projects</h2>
    <p>Drone</p>
    <p>Line Follower Bot</p>
   </section>
    <section id="contact">
        <h2>Contact</h2>
        <p>Email: <a href="user123@gmail.com">user123@gmail.com</a></p>
        <p>phone: <a href="phone:+915826578578">+915826578578</a>3@gmail.com</a></p>
    </section>
    <script>
        const projects = [
            { name: "UI/UX DESIGNER", description: "Well, known to design a web page in Figma, with the use of protypes,componnets and icon libraries.Ready to collaborate with companies."},

            { name: "TEAM HEAD", description: "I have worked as a team lead for the Team Robust Triumph and we built a self-made FPV drone. Which can be used for both racing and surveillance purposes.." }
        ];

        const projectContainer = document.getElementById("projects");
        projects.forEach(project => {
            let div = document.createElement("div");
            div.className = "project";
            div.innerHTML = `<h3>${project.name}</h3><p>${project.description}</p>`;
            projectContainer.appendChild(div);
        });
    </script>
</body>
</html>
