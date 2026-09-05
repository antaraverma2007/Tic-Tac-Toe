# 🎮 Tic-Tac-Toe Game

A simple and interactive **Tic-Tac-Toe game** built using **HTML, CSS, and JavaScript**. Two players can play against each other by taking turns as **O** and **X**.

The game automatically detects a winner or declares a draw when all boxes are filled.

## ✨ Features

* 🎯 Two-player gameplay
* 🔄 Alternating turns between O and X
* 🏆 Automatic winner detection
* 🤝 Draw detection
* 🔁 Reset Game button
* 🆕 New Game option after winning or drawing
* 🚫 Disables boxes after a move
* 📱 Responsive layout using CSS viewport units
* 🎨 Simple and clean UI

## 🛠️ Technologies Used

* **HTML5** – Structure of the game
* **CSS3** – Styling and responsive layout
* **JavaScript** – Game logic, winner detection, draw detection, and DOM manipulation

## 📂 Project Structure

```text
Tic-Tac-Toe/
│
├── index.html
├── style.css
├── app.js
└── README.md
```

## 🎮 How to Play

1. Open `index.html` in your browser.
2. Player O starts the game.
3. Players take turns clicking on an empty box.
4. The first player to get **three symbols in a row** wins.
5. If all 9 boxes are filled and nobody wins, the game ends in a **draw**.
6. Click **Reset Button** or **New Game** to play again.

## 🏆 Winning Patterns

A player wins by placing three identical symbols in:

* ➡️ A horizontal row
* ⬇️ A vertical column
* ↘️ A diagonal

Example:

```text
O | O | O
---------
X | X |  
---------
  |   |
```

Here, **O wins**.

## 🤝 Draw Condition

If all 9 boxes are filled and no player has a winning combination:

```text
X | O | X
---------
X | O | O
---------
O | X | X
```

The game displays:

```text
Game is a Draw!
```

## 🧠 JavaScript Logic

The game uses an array of winning patterns:

```javascript
const winPatterns = [
    [0,1,2],
    [0,3,6],
    [0,4,8],
    [1,4,7],
    [2,5,8],
    [2,4,6],
    [3,4,5],
    [6,7,8]
];
```

A `count` variable keeps track of the number of moves:

```javascript
let count = 0;
```

After every move:

```javascript
count++;
```

If all 9 boxes are filled without a winner:

```javascript
if(count === 9){
    msg.innerText = "Game is a Draw!";
}
```

## 🚀 Future Improvements

* 🤖 Add a single-player mode with AI
* 📊 Add score tracking
* 🔊 Add sound effects
* 🌙 Add dark mode
* 🎨 Add multiple themes
* 🏅 Add player names and scores

## 👩‍💻 Author

**Antara Verma**

Built as a frontend mini project while learning **HTML, CSS, and JavaScript**.
