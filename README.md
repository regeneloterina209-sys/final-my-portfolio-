<!DOCTYPE html>
<html>
<head>
    <title>Regene Loteriña | Portfolio</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <style>
        * {
            box-sizing: border-box;
        }

        body {
            margin: 0;
            font-family: Arial, sans-serif;
            background: #F5E8C8;
            color: #50391F;
        }

        .slide {
            display: none;
            min-height: 100vh;
            padding: 30px 20px;
            justify-content: center;
            align-items: center;
            text-align: center;
        }

        .active {
            display: flex;
        }

        .card {
            width: 100%;
            max-width: 550px;
            padding: 40px 25px;
            background: #FFF9EB;
            border-radius: 12px;
            border: 1px solid #D6BC80;
        }

        h1 {
            font-size: 36px;
            color: #76552E;
        }

        h2 {
            color: #8B6A35;
            font-size: 25px;
        }

        p {
            font-size: 18px;
            line-height: 1.7;
            color: #50391F;
        }

        .subtitle {
            color: #8B6A35;
            font-weight: bold;
            letter-spacing: 2px;
            font-size: 14px;
        }

        .project {
            background: #F5E8C8;
            padding: 20px;
            border-radius: 10px;
            margin: 20px 0;
            text-align: left;
        }

        button {
            background: #8B6A35;
            color: white;
            border: none;
            padding: 13px 28px;
            border-radius: 6px;
            margin: 15px 5px 0;
            font-size: 16px;
            cursor: pointer;
        }

        button:hover {
            background: #654821;
        }

        a {
            color: #76552E;
            font-weight: bold;
            overflow-wrap: anywhere;
        }

        .footer {
            font-size: 14px;
            color: #8B6A35;
            margin-top: 25px;
        }

        @media (max-width: 400px) {
            h1 {
                font-size: 29px;
            }

            p {
                font-size: 16px;
            }
        }
    </style>
</head>

<body>

    <!-- SLIDE 1: PORTFOLIO -->

    <section class="slide active">
        <div class="card">

            <p class="subtitle">WELCOME TO MY</p>

            <h1>MY PORTFOLIO</h1>

            <h2>REGENE LOTERIÑA</h2>

            <p>BSIT 1C</p>

            <p>
                A student exploring the world
                of technology and programming.
            </p>

            <button onclick="showSlide(1)">
                Next
            </button>

            <p class="footer">01 / 03</p>

        </div>
    </section>


    <!-- SLIDE 2: ABOUT ME -->

    <section class="slide">
        <div class="card">

            <p class="subtitle">GET TO KNOW ME</p>

            <h1>ABOUT ME</h1>

            <h2>Regene Loteriña</h2>

            <p>
                I am a first-year Bachelor of Science
                in Information Technology student
                from BSIT 1C.
            </p>

            <p>
                I am interested in learning about
                technology, programming, and
                computer systems.
            </p>

            <p>
                I am eager to develop my skills
                and gain more knowledge as
                I continue my studies.
            </p>

            <button onclick="showSlide(0)">
                Back
            </button>

            <button onclick="showSlide(2)">
                Next
            </button>

            <p class="footer">02 / 03</p>

        </div>
    </section>


    <!-- SLIDE 3: MY WORK AND CONTACT -->

    <section class="slide">
        <div class="card">

            <p class="subtitle">MY PROJECT</p>

            <h1>MY WORK</h1>

            <div class="project">

                <h2>Simple Calculator</h2>

                <p>
                    A basic calculator program
                    developed using Java.
                </p>

                <p>
                    It performs addition,
                    subtraction, multiplication,
                    and division.
                </p>

            </div>

            <h2>CONTACT INFORMATION</h2>

            <p>Email Address:</p>

            <p>
                <a href="mailto:regeneloterina209@email.com">
                    regeneloterina209@email.com
                </a>
            </p>

            <button onclick="showSlide(1)">
                Back
            </button>

            <button onclick="showSlide(0)">
                Home
            </button>

            <p class="footer">03 / 03</p>

        </div>
    </section>


    <!-- NAVIGATION SCRIPT -->

    <script>
        function showSlide(number) {

            let slides = document.querySelectorAll(".slide");

            slides.forEach(function(slide) {
                slide.classList.remove("active");
            });

            slides[number].classList.add("active");

            window.scrollTo(0, 0);
        }
    </script>

</body>
</html>
