
<!DOCTYPE html>
<html lang="uk">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Угадай число</title>
</head>
<body>
    <h1>Гра "Угадай число"</h1>
    <p>Угадай число від 1 до 100:</p>
    <input type="number" id="guess" min="1" max="100">
    <button onclick="checkGuess()">Перевірити</button>
    <p id="result"></p>

    <script>
        const randomNumber = Math.floor(Math.random() * 100) + 1;

        function checkGuess() {
            const userGuess = document.getElementById("guess").value;
            const result = document.getElementById("result");

            if (userGuess == randomNumber) {
                result.innerHTML = "Вітаю! Ви вгадали!";
            } else if (userGuess > randomNumber) {
                result.innerHTML = "Забагато! Спробуйте ще.";
            } else {
                result.innerHTML = "Замало! Спробуйте ще.";
            }
        }
    </script>
</body>
</html>
<!---
Vladidad/Vladidad is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
