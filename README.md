
<!DOCTYPE html>
<html lang="cs">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Učení je mučení</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            display: flex;
            min-height: 100vh;
            flex-direction: column;
        }

        header {
            background-color: #f0f0f0;
            padding: 1em;
            text-align: center;
        }

        .main-content {
            flex-grow: 1;
            display: flex;
            padding: 20px;
        }

        .article-section {
            flex-grow: 1;
            padding-right: 20px;
            overflow-y: auto; /* Zajistí srolování hlavní části */
        }

        .sidebar {
            width: 200px;
            padding: 20px;
            background-color: #e0e0e0;
        }

        .sidebar ul {
            list-style: none;
            padding: 0;
        }

        .sidebar li {
            margin-bottom: 10px;
        }

        .sidebar li a {
            text-decoration: none; /* Odstraní podtržení odkazů */
            color: #333; /* Nastaví barvu textu odkazu */
        }

        .sidebar li a:hover {
            color: blue; /* Změní barvu při najetí myší */
        }

        /* Pro dva boční panely */
        .left-sidebar {
            margin-right: 20px;
        }

        /* Pro rozložení se dvěma bočními panely */
        .main-content.two-sidebars {
            padding-left: 0;
            padding-right: 0;
        }

        .article-section.with-two-sidebars {
            padding-left: 20px;
            padding-right: 20px;
        }

        /* Styly pro kvíz */
        .quiz-container {
            margin-top: 20px;
            padding: 20px;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        .quiz-container .question {
            font-weight: bold;
            margin-bottom: 10px;
        }
        .quiz-container .options label {
            display: block;
            margin-bottom: 5px;
        }
        .quiz-container button {
            padding: 10px 15px;
            background-color: #007bff;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            margin-top: 10px;
        }
        .quiz-container .result {
            margin-top: 20px;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <header>
        <h1>Učení je mučení</h1>
    </header>

    <div class="main-content two-sidebars">
        <div class="left-sidebar sidebar">
            <h2>Matematika</h2>
            <ul>
                <li><a href="https://youtube.com/watch?v=fhe7WsRPDa0&feature=shared">Daniel</a></li>
                <li><a href="https://www.youtube.com/shorts/oLh0qNzXkMw">Zeman</a></li>
                <li><a href="https://www.example.com/karel">čeština</a></li>
                <li><a href="https://www.example.com/eva">fyzika</a></li>
                <li><a href="https://www.example.com/jana">přírodověda</a></li>
                <li><a href="https://www.example.com/michaela">zeměpis</a></li>
            </ul>
        </div>

        <div class="article-section with-two-sidebars">
            <h2>Tohle je pro tebe myšáku učit se, učit se! - </h2>
            <article>
                <h3>Matematika</h3>
                <p>Poměr je způsob, jak porovnávat údaje lépe než jen "větší, menší, rovno". V životě se s poměrem setkáte při zápisu výsledků sportovních zápasů, v návodu, jak ředit barvy, v receptech...</p>
            </article>
            <article>
                <h3>Čeština</h3>
                <p>Tady bude aktuální učivo ze sedmé třídy.</p>
            </article>

            <article class="quiz-container">
                <h3>Jednoduchý kvíz</h3>
                <div id="question-container"></div>
                <div id="options-container"></div>
                <button id="submit-btn">Odeslat odpověď</button>
                <div id="result-container" class="result" style="display: none;"></div>
            </article>

            <article>
                <h3>Fyzika</h3>
                <p>Gravitace je přírodní jev, který se projevuje jako vzájemné přitažlivé působení (interakci) všech objektů, které mají hmotnost nebo energii..</p>
            </article>
            <article>
                <h3>Zeměpis</h3>
                <p>Země je v některých evropských státech označení pro existující či historické vyšší územní jednotky zpravidla většího rozsahu a vybavené velkou mírou samosprávy nebo přímo autonomií (vlastním parlamentem, vládou, legislativou apod.). Stát se pak zpravidla z takových zemí skládá i administrativně.

V řadě států se pro obdobné správní celky užívají jiné pojmy stejného významu, např. ve Švýcarsku kantony, ve Španělsku autonomní společenství, někde provincie (v Kanadě, v Jihoafrické republice), někde svazový/spolkový stát nebo stát unie/federace (často uváděný jen jako „stát“), např. v USA, Indii, Brazílii, Malajsii nebo Austrálii. V Ruské federaci se celky na této úrovni nazývají republiky (nejsou však skladebné – nepokrývají celé území státu), na republiky se členila i Jugoslávie..</p>
            </article>
            <article>
                <h3>Dějepis</h3>
                <p>Karel IV., narozen jako Václav, byl jedenáctý český král vládnoucí jako Karel I. od srpna 1346 až do své smrti v listopadu 1378. Karel IV. byl římsko-německý král od července 1346 a od roku 1355 císař římský. </p>
            </article>
            <article>
                <h3>Článek 6</h3>
                <p>Ještě nevím.</p>
            </article>
        </div>

        <div class="right-sidebar sidebar">
            <h2>Odkazy vpravo</h2>
            <ul>
                <li><a href="https://https://youtu.be/fhe7WsRPDa0?si=fO_KskV6OsiyuXOb">Alfa</a></li>
                <li><a href="https://www.example.com/beta">Beta</a></li>
                <li><a href="https://www.example.com/gamma">Gama</a></li>
                <li><a href="https://www.example.com/delta">Delta</a></li>
                <li><a href="https://www.example.com/epsilon">Epsilon</a></li>
                <li><a href="https://www.example.com/zeta">Zeta</a></li>
            </ul>
        </div>
    </div>

    <footer>
        <p>© 2023 Moje stránka</p>
    </footer>

    <script>
        const questions = [
            {
                question: "Kolik je 2 + 2?",
                options: ["3", "4", "5", "6"],
                correctAnswer: "4"
            },
            {
                question: "Jaká je hlavní město České republiky?",
                options: ["Brno", "Ostrava", "Praha", "Plzeň"],
                correctAnswer: "Praha"
            },
            {
                question: "Kdo napsal knihu Malý princ?",
                options: ["Antoine de Saint-Exupéry", "J.R.R. Tolkien", "Lewis Carroll", "Hans Christian Andersen"],
                correctAnswer: "Antoine de Saint-Exupéry"
            }
        ];

        let currentQuestionIndex = 0;
        let score = 0;

        const questionContainer = document.getElementById("question-container");
        const optionsContainer = document.getElementById("options-container");
        const submitBtn = document.getElementById("submit-btn");
        const resultContainer = document.getElementById("result-container");

        function displayQuestion() {
            const currentQuestion = questions[currentQuestionIndex];
            questionContainer.textContent = currentQuestion.question;
            optionsContainer.innerHTML = ""; // Vyčistí předchozí možnosti

            currentQuestion.options.forEach((option, index) => {
                const label = document.createElement("label");
                const radioBtn = document.createElement("input");
                radioBtn.type = "radio";
                radioBtn.name = "answer";
                radioBtn.value = option;
                label.appendChild(radioBtn);
                label.appendChild(document.createTextNode(option));
                optionsContainer.appendChild(label);
            });
        }

        function checkAnswer() {
            const selectedOption = document.querySelector('input[name="answer"]:checked');
            if (selectedOption) {
                if (selectedOption.value === questions[currentQuestionIndex].correctAnswer) {
                    score++;
                }
                currentQuestionIndex++;

                if (currentQuestionIndex < questions.length) {
                    displayQuestion();
                } else {
                    showResult();
                }
            } else {
                alert("Prosím, vyberte odpověď!");
            }
        }

        function showResult() {
            questionContainer.style.display = "none";
            optionsContainer.style.display = "none";
            submitBtn.style.display = "none";
            resultContainer.textContent = `Tvůj výsledek: ${score} z ${questions.length} správně!`;
            resultContainer.style.display = "block";
        }

        submitBtn.addEventListener("click", checkAnswer);

        displayQuestion(); // Zobrazí první otázku při načtení stránky
    </script>
</body>
</html>
