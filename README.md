# guesstheno
🎯 Number Guessing Game
A fun and interactive browser-based number guessing game built with pure HTML, CSS, and JavaScript — no libraries or frameworks needed!
---
📸 Preview
> Open `index.html` in any browser to play instantly!
---
📁 Project Structure
```
number-guessing-game/
├── index.html       ← Page structure (buttons, input, layout)
├── style.css        ← All visual styling (colors, fonts, animations)
├── script.js        ← Game logic (random number, guessing, score)
└── README.md        ← You are here!
```
---
🎮 How to Play
The computer secretly picks a random number between 1 and 100
Type your guess in the input box and click Guess! (or press Enter)
You'll get a hint after every guess:
📈 Too High — your guess is above the secret number
📉 Too Low — your guess is below the secret number
🎉 Correct! — you found it!
Try to guess it in as few attempts as possible
Click 🔄 Restart Game to play again
---
✅ Features
🎲 Random number generated between 1 and 100
💬 Real-time feedback: Too High / Too Low / Correct
🔢 Attempt counter displayed after every guess
🏷️ Colour-coded guess history chips (↑ too high, ↓ too low, ✓ correct)
⌨️ Press Enter to submit a guess (no need to click)
✅ Input validation — rejects invalid or out-of-range numbers
🔄 Restart button to begin a new game instantly
🌙 Stylish dark UI with gradient accents
---
🚀 How to Run
Option 1 — Open directly in browser (easiest)
Download all 4 files into the same folder
Double-click `index.html`
The game opens in your browser — no installation needed!
Option 2 — Use VS Code Live Server
Install VS Code
Install the Live Server extension
Right-click `index.html` → Open with Live Server
---
🛠️ Built With
Technology	Purpose
HTML5	Page structure and layout
CSS3	Styling, animations, responsive design
JavaScript (ES6)	Game logic, DOM manipulation
Google Fonts	Boogaloo + Nunito typefaces
---
🔮 Future Improvements
#	Feature	Difficulty	Priority
G-1	Difficulty levels (Easy / Medium / Hard)	Easy	High
G-2	Limited attempts mode (10 guesses max)	Easy	High
G-3	Hint system after 3 wrong guesses	Medium	Medium
G-4	Time Attack mode with countdown timer	Medium	Medium
S-1	High score saved in localStorage	Easy	High
S-2	Score based on attempts + time	Easy	Medium
S-3	Top 5 leaderboard	Medium	Medium
U-1	Sound effects (Web Audio API)	Easy	Medium
U-2	Confetti animation on win	Easy	Medium
U-3	Warm / Cold proximity bar	Medium	High
U-4	Light / Dark mode toggle	Easy	Medium
U-5	Accessibility improvements (ARIA)	Medium	High
U-6	Mobile-responsive layout	Easy	High
T-1	Custom number range (user defined)	Easy	Medium
T-4	Unit tests with Jest	Medium	Medium
---
📖 Code Explanation (For Beginners)
How the random number is generated (`script.js`)
```js
secretNumber = Math.floor(Math.random() * 100) + 1;
```
`Math.random()` → gives a decimal like `0.73`
`* 100` → makes it `73.0`
`Math.floor()` → rounds down to `73`
`+ 1` → shifts the range from 0–99 to 1–100
How the guess is checked
```js
if (guess > secretNumber)  // Too High
if (guess < secretNumber)  // Too Low
if (guess === secretNumber) // Correct!
```
How the attempt counter works
```js
attempts++; // Adds 1 every time the player makes a valid guess
```
---
🤝 How to Contribute
Download or fork the project
Pick a feature from the Future Improvements table
Edit the files in any code editor (VS Code recommended)
Test by opening `index.html` in your browser
Share your improved version!
---
📄 License
This project is open source and free to use for learning purposes.
---
👨‍💻 Author
Built as a beginner HTML + CSS + JavaScript project.  
Happy coding! 🎉
