# ♟️ Chess With AI Opponents

A browser-based chess game built in React and TypeScript, featuring homemade AI opponents. The chess logic—including all movement, rules, and simple AI—was coded from scratch with no outside chess or AI libraries. This project is both a programming exercise and a demonstration of my understanding of chess mechanics and modern web app development.

---

## 🚀 Demo

Play it now: [GitHub Pages Live Demo](https://cmac2112.github.io/Chess-With-AI-Opponents/home)

---

## Features

- **Full Chess Game**: All core chess rules implemented, including pawn promotion, check/checkmate, and legal moves.
- **AI Opponents**: Play against the computer at multiple difficulty levels. AI logic is custom-made—no external chess or AI engines are used.
- **Modern UI**: Responsive design with React, piece movement, and game status displays.
- **Singleplayer**: Play against yourself or challenge the built-in AI.
- **From Scratch Logic**: All move generation and game rules are implemented in TypeScript. no chess logic libraries were used.
- **Customizable**: Easily extendable to add new features or change AI difficulty.

---

## How It Works

- The board and pieces are represented as JavaScript arrays and strings.
- All move validation, check/checkmate detection, and rule enforcement is handled with original functions.
- The AI makes its decisions using hand-coded logic that evaluates possible moves and picks one based on a basic point-scoring system (see `chessjs/src/Utilities/AICalculation.tsx`).
- No outside chess (e.g., `chess.js`, Stockfish, etc.) or AI libraries—everything is coded by hand!

---

## Project Structure

```
Chess-With-AI-Opponents/
  chessjs/
    src/
      components/       # React components like Box (board square)
      Utilities/        # All chess and AI logic (hand-written)
      pages/            # Main pages (Home/game UI)
      App.tsx           # Entry and router
      index.css         # Main styling
      ...
    public/
    package.json        # React, Vite, ESLint, TypeScript, React Router
    vite.config.ts
    ...
  README.md
```

---

## Setup & Running Locally

1. **Clone the project:**
   ```bash
   git clone https://github.com/cmac2112/Chess-With-AI-Opponents.git
   cd Chess-With-AI-Opponents/chessjs
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Start the development server:**
   ```bash
   npm run dev
   ```

   Then visit [`http://localhost:5173`](http://localhost:5173).

4. **Build for production:**
   ```bash
   npm run build
   ```

---

## Custom AI and Game Logic

All AI and chess mechanics use original algorithms coded in TypeScript for learning purposes.
- **AI**: Logic lives in [`/src/Utilities/AICalculation.tsx`](chessjs/src/Utilities/AICalculation.tsx) and always plays as black. The "easy" mode picks moves based on maximizing captured piece value.
- **Chess rules**: Movement and validation functions are hand-written and live in [`/src/Utilities/Utilities.tsx`](chessjs/src/Utilities/Utilities.tsx).

**No chess.js, Stockfish, minimax packages, or other outside engines!**

---

## Why?

This project was created to learn:
- How to develop a full chess engine with piece movement, detection of check, checkmate, and game validation from scratch
- Core React and TypeScript skills
- How to architect a small game in a modern web stack

---

## Issues & Contributing

Have an idea or see a bug? Open an issue or pull request!
- See the [Issues page](https://github.com/cmac2112/Chess-With-AI-Opponents/issues) for current work and ideas.

---

## License

MIT

---

Enjoy playing, learning, and hacking!

<br>
<sub>“All logic is original and coded by hand—no outside packages for chess or AI logic are used.”</sub>
