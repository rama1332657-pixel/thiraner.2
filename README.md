<!DOCTYPE html>
<html>
<head>
    <title>Advanced CSS3 Responsive Portfolio</title>

    <style>
        /* CSS Variables */
        :root {
            --bg-color: #ffffff;
            --text-color: #333;
            --main-color: #0066ff;
            --card-color: #f2f2f2;
        }

        /* Basic Style */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Arial, sans-serif;
        }

        body {
            background: var(--bg-color);
            color: var(--text-color);
        }

        /* Flexbox Header */
        header {
            background: var(--main-color);
            color: white;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 40px;
        }

        nav a {
            color: white;
            text-decoration: none;
            margin-left: 15px;
            font-weight: bold;
        }

        /* Hero Section */
        .hero {
            text-align: center;
            padding: 70px 20px;
        }

        .hero h2 {
            font-size: 35px;
            margin-bottom: 15px;
        }

        .hero p {
            font-size: 18px;
            margin-bottom: 20px;
        }

        button {
            background: var(--main-color);
            color: white;
            border: none;
            padding: 12px 25px;
            border-radius: 5px;
            cursor: pointer;
        }

        button:hover {
            background: #004bcc;
        }

        /* CSS Grid */
        .grid-container {
            display: grid;
            grid-template-columns: 1fr;
            gap: 20px;
            padding: 20px;
        }

        .card {
            background: var(--card-color);
            padding: 25px;
            border-radius: 10px;
            text-align: center;
            box-shadow: 0 2px 8px gray;
        }

        /* Tablet View */
        @media (min-width: 768px) {
            .grid-container {
                grid-template-columns: repeat(2, 1fr);
            }
        }

        /* Desktop View */
        @media (min-width: 1024px) {
            .grid-container {
                grid-template-columns: repeat(3, 1fr);
            }
        }

        footer {
            background: var(--main-color);
            color: white;
            text-align: center;
            padding: 15px;
            margin-top: 20px;
        }
    </style>

</head>

<body>

    <header>
        <h1>My Portfolio</h1>

        <nav>
            <a href="#">Home</a>
            <a href="#">About</a>
            <a href="#">Skills</a>
            <a href="#">Contact</a>
        </nav>
    </header>


    <section class="hero">
        <h2>Hello, I am a Web Developer</h2>
        <p>
            I create modern responsive websites using HTML5 and CSS3.
        </p>

        <button>View My Work</button>
    </section>


    <section class="grid-container">

        <div class="card">
            <h2>About Me</h2>
            <p>
                I am a passionate developer interested in creating websites.
            </p>
        </div>

        <div class="card">
            <h2>Skills</h2>
            <p>
                HTML, CSS3, Java, Python and Responsive Web Design.
            </p>
        </div>

        <div class="card">
            <h2>Projects</h2>
            <p>
                Portfolio websites, applications and software projects.
            </p>
        </div>

    </section>


    <footer>
        <p>© 2026 My Responsive Portfolio</p>
    </footer>

</body>
</html>
