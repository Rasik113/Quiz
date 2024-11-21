<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Quiz Competition</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 20px;
            line-height: 1.6;
        }
        .round {
            margin-bottom: 30px;
        }
        .round-title {
            font-size: 1.5em;
            margin-bottom: 10px;
        }
        .question-list, .categories {
            list-style-type: none;
            padding: 0;
        }
        .question-list li, .categories li {
            margin: 5px 0;
        }
        .categories {
            margin-top: 10px;
        }
        .difficulty {
            margin-left: 20px;
        }
        .reveal-btn {
            display: none;
            margin-top: 5px;
            cursor: pointer;
        }
    </style>
    <script>
        function revealAnswer(btn, answer) {
            btn.previousElementSibling.textContent = answer;
            btn.style.display = "none";
        }
    </script>
</head>
<body>
    <h1>Quiz Competition</h1>
    <div class="round">
        <div class="round-title">Regular Round</div>
        <ul class="question-list">
            <li>
                <a href="reguralRound/regular-q1.html">Question 1</a>
                <div class="reveal-btn-container">
                </div>
            </li>
        </ul>
    </div>
    <div class="round">
        <div class="round-title">Buzzer Round</div>
        <ul class="question-list">
            <li>
                <a href="#buzzer-q1">Question 1</a>
                <div class="reveal-btn-container">
                    <span></span>
                    <button class="reveal-btn" onclick="revealAnswer(this, 'Answer 1')">Reveal Answer</button>
                </div>
            </li>
        </ul>
    </div>
    <div class="round">
        <div class="round-title">Rapid Fire Round</div>
        <ul class="question-list">
            <li>
                <a href="#rapid-q1">Question 1</a>
                <div class="reveal-btn-container">
                    <span></span>
                    <button class="reveal-btn" onclick="revealAnswer(this, 'Answer 1')">Reveal Answer</button>
                </div>
            </li>
        </ul>
    </div>
    <div class="round">
        <div class="round-title">Selection Round</div>
        <ul class="categories">
            <li>Geography
                <ul class="difficulty">
                    <li><a href="#geo-q100">100 Points</a></li>
                    <li><a href="#geo-q200">200 Points</a></li>
                    <li><a href="#geo-q300">300 Points</a></li>
                    <li><a href="#geo-q400">400 Points</a></li>
                    <li><a href="#geo-q500">500 Points</a></li>
                </ul>
            </li>
            <li>Physics
                <ul class="difficulty">
                    <li><a href="#phy-q100">100 Points</a></li>
                    <li><a href="#phy-q200">200 Points</a></li>
                    <li><a href="#phy-q300">300 Points</a></li>
                    <li><a href="#phy-q400">400 Points</a></li>
                    <li><a href="#phy-q500">500 Points</a></li>
                </ul>
            </li>
            <li>Mathematics
                <ul class="difficulty">
                    <li><a href="#math-q100">100 Points</a></li>
                    <li><a href="#math-q200">200 Points</a></li>
                    <li><a href="#math-q300">300 Points</a></li>
                    <li><a href="#math-q400">400 Points</a></li>
                    <li><a href="#math-q500">500 Points</a></li>
                </ul>
            </li>
        </ul>
    </div>
</body>
</html>
