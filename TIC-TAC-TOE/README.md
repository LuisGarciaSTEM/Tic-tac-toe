# Tic-Tac-Toe Game

This is a simple implementation of the classic Tic-Tac-Toe game using React.

## Features

- Two-player game (X and O)
- Keeps track of game history
- Allows players to jump to previous moves
- Displays the winner

## Getting Started

### Prerequisites

- Node.js
- npm (Node Package Manager)

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/Tic-tac-toe.git
   ```
2. Navigate to the project directory:
   ```bash
   cd Tic-tac-toe
   ```
3. Install the dependencies:
   ```bash
   npm install
   ```

### Running the Game

To start the development server and play the game, run:
```bash
npm start
```
Open your browser and go to `http://localhost:3000` to see the game in action.

## Project Structure

```
Tic-tac-toe/
├── public/
│   ├── index.html
│   └── ...
├── src/
│   ├── App.jsx
│   ├── App.css
│   ├── index.css
│   └── ...
├── package.json
└── README.md
```

- `src/App.jsx`: Contains the main game logic and components.
- `src/App.css`: Contains the CSS styles specific to the game.
- `src/index.css`: Contains global CSS styles.

## Components

### Square

Renders a single square button.

```jsx
function Square({ value, onSquareClick }) {
  return (
    <button className="square" onClick={onSquareClick}>
      {value}
    </button>
  );
}
```

### Board

Renders the game board and handles game logic.

```jsx
function Board({ xIsNext, squares, onPlay }) {
  // ...existing code...
}
```

### Game

Manages the state of the game and renders the board and game history.

```jsx
export default function Game() {
  // ...existing code...
}
```

## Helper Functions

### calculateWinner

Determines the winner of the game.

```jsx
function calculateWinner(squares) {
  // ...existing code...
}
```

## CSS

### App.css

Contains the CSS styles specific to the game.

```css
/* ...existing code... */
```

### index.css

Contains global CSS styles.

```css
/* ...existing code... */
```

## License

This project is licensed under the MIT License.
