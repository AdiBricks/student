---
title: Number Picker Game
layout: post
description: A pretty not advanced use of JavaScript building classic number generation game using menu controls, key events, snake simulation and timers.  
courses: { csp: {week: 1}}
type: hacks
---

<html>
<head>
    <title>Guess the Number (1-100)</title>
    <style>
        body {
            text-align: center;
            font-family: Arial, sans-serif;
        }
    </style>
</head>
<body>
    <h1>Guess the Number (1-100)</h1>
    <p>Try to guess the correct number between 1 and 100.</p>
    <input type="number" id="guess" placeholder="Enter your guess">
    <button onclick="checkGuess()">Submit Guess</button>
    <p id="message"></p>

    <script>
        // Generate a random number between 1 and 100
        const randomNumber = Math.floor(Math.random() * 100) + 1;
        let attempts = 0;

        function checkGuess() {
            const guess = parseInt(document.getElementById('guess').value);
            attempts++;

            if (guess === randomNumber) {
                document.getElementById('message').textContent = `Congratulations! You guessed the number ${randomNumber} in ${attempts} attempts.`;
            } else if (guess < randomNumber) {
                document.getElementById('message').textContent = 'Try a higher number.';
            } else {
                document.getElementById('message').textContent = 'Try a lower number.';
            }
        }
    </script>
</body>
</html>
