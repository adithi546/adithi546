<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Quiz</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #f0f0f0;
            margin: 0;
            padding: 0;
        }
        .quiz-container {
            max-width: 600px;
            margin: 20px auto;
            background-color: #fff;
            border-radius: 10px;
            padding: 20px;
            box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.2);
        }
        h1 {
            font-size: 24px;
        }
        .question {
            font-size: 18px;
            margin-bottom: 20px;
        }
        .options {
            display: flex;
            flex-direction: column;
            align-items: flex-start;
        }
        .option {
            cursor: pointer;
            padding: 10px;
            border: 1px solid #ccc;
            border-radius: 5px;
            margin-bottom: 10px;
            transition: background-color 0.3s, color 0.3s;
        }
        .option:hover {
            background-color: #f0f0f0;
        }
        .option.selected {
            background-color: #007bff;
            color: #fff;
        }
        #submit-btn {
            background-color: #007bff;
            color: #fff;
            border: none;
            border-radius: 5px;
            padding: 10px 20px;
            font-size: 16px;
            cursor: pointer;
            transition: background-color 0.3s, color 0.3s;
        }
        #submit-btn:hover {
            background-color: #0056b3;
        }
        #score {
            font-size: 20px;
            margin-top: 20px;
        }
        #timer {
            font-size: 16px;
            margin-top: 10px;
        }
    </style>
</head>
<body>
    <div class="quiz-container">
        <h1>Interactive Quiz</h1>
        <div class="question" id="question"></div>
        <div class="options" id="options"></div>
        <div id="timer">Time Left: <span id="time-left"></span> seconds</div>
        <button id="submit-btn" disabled>Submit</button>
        <div id="score"></div>
        <button id="restart-btn" style="display: none;">Restart Quiz</button>
    </div>

    <script>
        const questions = [
            {
                question: " What company makes the Xperia model of smartphone?",
                options: ["Sony","Samsung","Nokia","One plus"],
                correctAnswer: "Sony"
            },
            {
                question: "Who is generally considered the inventor of the motor car?",
                options: ["Henry Ford", "Karl Benz", "Henry M. Leland", "Roger Daltrey"],
                correctAnswer: "Karl Benz"
            },
            {
                question: " What is the largest US state (by landmass)?",
                options: ["Texas", "Alaska", "California", "Florida"],
                correctAnswer: "Alaska"
            },
        ];

        let currentQuestion = 0;
        let score = 0;
        let timeLeft = 10; // Initial time for each question in seconds
        let timerInterval;

        const questionElem = document.getElementById('question');
        const optionsElem = document.getElementById('options');
        const submitBtn = document.getElementById('submit-btn');
        const scoreElem = document.getElementById('score');
        const restartBtn = document.getElementById('restart-btn');
        const timeLeftElem = document.getElementById('time-left');

        function loadQuestion() {
            clearInterval(timerInterval);
            timeLeft = 10; // Reset the timer for each question
            updateTimeLeft();
            
            const current = questions[currentQuestion];
            questionElem.textContent = current.question;
            optionsElem.innerHTML = '';
            current.options.forEach((option, index) => {
                const optionElem = document.createElement('div');
                optionElem.textContent = option;
                optionElem.classList.add('option');
                optionElem.addEventListener('click', () => selectAnswer(option, index));
                optionsElem.appendChild(optionElem);
            });

            // Start the timer
            timerInterval = setInterval(() => {
                timeLeft--;
                updateTimeLeft();
                if (timeLeft <= 0) {
                    // Time's up, automatically submit
                    clearInterval(timerInterval);
                    selectAnswer(null, -1); // Pass -1 as an index to indicate timeout
                }
            }, 1000);
        }

        function updateTimeLeft() {
            timeLeftElem.textContent = timeLeft;
        }

        function selectAnswer(selectedOption, selectedIndex) {
            clearInterval(timerInterval);

            if (selectedOption !== null) {
                const current = questions[currentQuestion];
                const options = optionsElem.querySelectorAll('.option');
                options.forEach((option, index) => {
                    option.classList.remove('selected');
                    if (index === selectedIndex) {
                        option.classList.add('selected');
                    }
                });

                if (selectedOption === current.correctAnswer) {
                    score++;
                }
            }

            submitBtn.disabled = false;
        }

        function showScore() {
            questionElem.textContent = `Quiz completed! Your Score: ${score} out of ${questions.length}`;
            optionsElem.innerHTML = '';
            submitBtn.style.display = 'none';
            scoreElem.textContent = '';
            restartBtn.style.display = 'block';
        }

        function restartQuiz() {
            currentQuestion = 0;
            score = 0;
            loadQuestion();
            submitBtn.disabled = true;
            scoreElem.textContent = '';
            restartBtn.style.display = 'none';
        }

        submitBtn.addEventListener('click', () => {
            currentQuestion++;
            if (currentQuestion < questions.length) {
                loadQuestion();
                submitBtn.disabled = true;
            } else {
                // Quiz completed
                showScore();
            }
        });

        restartBtn.addEventListener('click', restartQuiz);

        loadQuestion();
    </script>
</body>
</html>
