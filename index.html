
<!DOCTYPE html>
<html lang="sv">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AI för lärare och pedagoger - Quiz</title>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/jspdf/2.5.1/jspdf.umd.min.js"></script>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            color: #333;
            max-width: 800px;
            margin: 0 auto;
            padding: 20px;
        }
        h1, h2 {
            color: #2c3e50;
        }
        .quiz-container {
            background-color: #f9f9f9;
            border-radius: 8px;
            padding: 20px;
            margin-top: 20px;
        }
        .question {
            margin-bottom: 20px;
        }
        .options {
            display: flex;
            flex-direction: column;
        }
        .option {
            margin: 5px 0;
            padding: 10px;
            background-color: #e0e0e0;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            transition: background-color 0.3s;
        }
        .option:hover {
            background-color: #d0d0d0;
        }
        .option.selected {
            background-color: #3498db;
            color: white;
        }
        .btn {
            padding: 10px 20px;
            background-color: #2ecc71;
            color: white;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            font-size: 16px;
            margin-top: 10px;
        }
        .btn:hover {
            background-color: #27ae60;
        }
        .result {
            font-weight: bold;
            font-size: 18px;
            margin-top: 20px;
        }
        .hidden {
            display: none;
        }
        input[type="text"] {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
            border: 1px solid #ddd;
            border-radius: 4px;
        }
        @media (max-width: 600px) {
            body {
                padding: 10px;
            }
            .quiz-container {
                padding: 10px;
            }
        }
    </style>
</head>
<body>
    <div class="quiz-container">
        <div id="start-screen">
            <h1>Välkommen till Quiz: AI för lärare och pedagoger</h1>
            <p>Testa dina kunskaper om AI i undervisningen!</p>
            <button class="btn" onclick="startQuiz()">Starta Quiz</button>
        </div>
        <div id="quiz-screen" class="hidden">
            <h2 id="question"></h2>
            <div id="options" class="options"></div>
            <button class="btn" onclick="nextQuestion()">Nästa fråga</button>
        </div>
        <div id="name-screen" class="hidden">
            <h2>Grattis! Du har klarat quizen.</h2>
            <p>Vänligen fyll i ditt namn för att få ditt diplom.</p>
            <input type="text" id="firstName" placeholder="Förnamn">
            <input type="text" id="lastName" placeholder="Efternamn">
            <button class="btn" onclick="showResult()">Visa resultat</button>
        </div>
        <div id="result-screen" class="hidden">
            <h2>Quiz Resultat</h2>
            <p id="score"></p>
            <p id="passFail"></p>
            <button class="btn" id="downloadBtn" onclick="generatePDF()">Ladda ner Diplom</button>
            <button class="btn" onclick="restartQuiz()">Börja om</button>
        </div>
    </div>

    <script>
        const quizData = [
            {
                question: "Varför är det viktigt att regelbundet granska hur AI-system påverkar olika elevgrupper?",
                options: [
                    "För att säkerställa rättvis och jämlik behandling av alla elever",
                    "För att öka användningen av AI i klassrummet",
                    "För att minska lärarnas arbetsbörda"
                ],
                correct: 0
            },
            {
                question: "Vilka försiktighetsåtgärder bör vidtas när man använder AI-verktyg som kan påverka betyg eller andra viktiga beslut?",
                options: [
                    "Använda AI-verktyg utan granskning",
                    "Vara extra noggrann och dubbelkolla AI-genererade bedömningar",
                    "Låta AI fatta alla beslut autonomt"
                ],
                correct: 1
            },
            {
                question: "Hur kan man integrera dataskydd i undervisningen när man använder AI?",
                options: [
                    "Ignorera dataskyddsfrågor helt",
                    "Lära ut vikten av dataskydd som en del av digital kompetens",
                    "Dela all elevinformation fritt med AI-system"
                ],
                correct: 1
            },
            {
                question: "Varför är det viktigt att vara transparent med användningen av AI i klassrummet?",
                options: [
                    "För att öka förvirringen kring AI",
                    "För att göra undervisningen mer komplicerad",
                    "För att göra AI begripligt och skapa förtroende hos elever och föräldrar"
                ],
                correct: 2
            },
            {
                question: "Hur kan AI användas för att stödja elever med olika behov och förutsättningar?",
                options: [
                    "Genom att behandla alla elever exakt likadant",
                    "Genom att utforska hur AI kan anpassas för olika elevers behov",
                    "Genom att exkludera vissa elever från AI-användning"
                ],
                correct: 1
            },
            {
                question: "Vilka grundläggande cybersäkerhetsprinciper bör läras ut i samband med AI-användning?",
                options: [
                    "Att dela lösenord fritt",
                    "Att ignorera säkerhetsvarningar",
                    "Att rapportera problem och följa säkerhetsrutiner"
                ],
                correct: 2
            },
            {
                question: "Beskriv skillnaden mellan att använda AI som ett pedagogiskt komplement och att låta AI ersätta läraren.",
                options: [
                    "Det finns ingen skillnad",
                    "AI bör helt ersätta läraren",
                    "AI används som stöd, men läraren styr undervisningen med sin expertis"
                ],
                correct: 2
            },
            {
                question: "Varför är det viktigt att utvärdera nya AI-verktyg i liten skala innan de implementeras fullt ut?",
                options: [
                    "För att fördröja implementeringen",
                    "För att noggrant bedöma verktygets påverkan på undervisning och lärande",
                    "För att göra eleverna frustrerade"
                ],
                correct: 1
            },
            {
                question: "Vilka riktlinjer bör finnas för elevers användning av AI i skolarbeten?",
                options: [
                    "Inga riktlinjer behövs",
                    "Förbjuda all användning av AI",
                    "Skapa tydliga riktlinjer för när och hur AI får användas, samt korrekt citering"
                ],
                correct: 2
            },
            {
                question: "Hur kan lärare uppmuntra kritiskt tänkande kring AI och dess resultat?",
                options: [
                    "Genom att acceptera alla AI-resultat utan ifrågasättande",
                    "Genom att förbjuda all diskussion om AI",
                    "Genom att uppmuntra elever att ifrågasätta och utvärdera AI-genererade resultat"
                ],
                correct: 2
            }
        ];

        let currentQuestion = 0;
        let score = 0;
        let selectedOption = -1;

        function startQuiz() {
            document.getElementById('start-screen').classList.add('hidden');
            document.getElementById('quiz-screen').classList.remove('hidden');
            loadQuestion();
        }

        function loadQuestion() {
            const question = quizData[currentQuestion];
            document.getElementById('question').textContent = question.question;
            const optionsContainer = document.getElementById('options');
            optionsContainer.innerHTML = '';
            question.options.forEach((option, index) => {
                const button = document.createElement('button');
                button.textContent = option;
                button.classList.add('option');
                button.onclick = () => selectOption(index);
                optionsContainer.appendChild(button);
            });
            selectedOption = -1;
        }

        function selectOption(index) {
            const options = document.querySelectorAll('.option');
            options.forEach(option => option.classList.remove('selected'));
            options[index].classList.add('selected');
            selectedOption = index;
        }

        function nextQuestion() {
            if (selectedOption === quizData[currentQuestion].correct) {
                score += 3;
            }
            currentQuestion++;
            if (currentQuestion < quizData.length) {
                loadQuestion();
            } else {
                if ((score / (quizData.length * 3)) > 0.8) {
                    document.getElementById('quiz-screen').classList.add('hidden');
                    document.getElementById('name-screen').classList.remove('hidden');
                } else {
                    showResult();
                }
            }
        }

        function showResult() {
            document.getElementById('quiz-screen').classList.add('hidden');
            document.getElementById('name-screen').classList.add('hidden');
            document.getElementById('result-screen').classList.remove('hidden');
            const scorePercentage = (score / (quizData.length * 3)) * 100;
            document.getElementById('score').textContent = `Du fick ${score} poäng av ${quizData.length * 3} möjliga (${scorePercentage.toFixed(1)}%).`;
            if (scorePercentage > 80) {
                document.getElementById('passFail').textContent = 'Grattis! Du har klarat quizen.';
                document.getElementById('downloadBtn').style.display = 'inline-block';
            } else {
                document.getElementById('passFail').textContent = 'Tyvärr, du behöver minst 80% rätt för att klara quizen. Försök igen!';
                document.getElementById('downloadBtn').style.display = 'none';
            }
        }

        function generatePDF() {
            const { jsPDF } = window.jspdf;
            const doc = new jsPDF();
            const firstName = document.getElementById('firstName').value;
            const lastName = document.getElementById('lastName').value;

            doc.setFontSize(24);
            doc.text('Diplom', 105, 20, null, null, 'center');
            
            doc.setFontSize(16);
            doc.text(`Detta intygar att`, 105, 40, null, null, 'center');
            
            doc.setFontSize(22);
            doc.text(`${firstName} ${lastName}`, 105, 55, null, null, 'center');
            
            doc.setFontSize(16);
            doc.text(`har framgångsrikt genomfört quizen`, 105, 70, null, null, 'center');
            doc.text(`"AI för lärare och pedagoger"`, 105, 80, null, null, 'center');
            doc.text(`med en poäng på ${score} av ${quizData.length * 3}`, 105, 90, null, null, 'center');

            const today = new Date();
            const dateString = today.toLocaleDateString('sv-SE');
            doc.text(`Datum: ${dateString}`, 105, 110, null, null, 'center');

            doc.save('AI_Quiz_Diplom.pdf');
        }

        function restartQuiz() {
            currentQuestion = 0;
            score = 0;
            document.getElementById('result-screen').classList.add('hidden');
            document.getElementById('start-screen').classList.remove('hidden');
        }
    </script>
</body>
</html>
