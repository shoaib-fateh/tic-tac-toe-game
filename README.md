# Tic-Tac-Toe Game

This is a simple yet sophisticated Tic-Tac-Toe game application developed with React.js. The game keeps track of the player's moves and records the history of gameplay, allowing players to revisit previous game states.

## Application Structure

The application is divided into three main components: Square, Board, and Game. 

- **Square Component:** This is the individual square of the Tic-Tac-Toe board, where a player chooses to place their 'X' or 'O'. It receives its current value ('X', 'O', or null) and a function to handle a player's click as props.

- **Board Component:** The Board represents the game board with nine squares. It maintains the current game status and handles any changes on the board, such as a player marking a square.

- **Game Component:** This is the root component that encapsulates the entire game. It initializes the game history as a state and manages the current move. 

## Gameplay

The gameplay rotates between two players, allowing them to place an 'X' or 'O' on the board in turns. When a player succeeds in placing three of their marks in a horizontal, vertical, or diagonal row, they win. The game also allows players to revisit a past board state by jumping to a specific move in history.

## Dependency 

The application state is managed using the useState React Hook to make it a fully functional interactive game with minimal, clean code.

## Usage

To run this project, first clone the repository, then navigate to the project directory and run `npm install` to install the dependencies. Start the game with `npm start`. 

[Launch App](https://tictac-toe-v2.netlify.app/){:target="_blank"}

## Future Enhancements

- Add a feature for the game to be played between a human and a computer.
- Indicate when a draw occurs if no player wins.
- Highlight the winning row when a player wins. 

This project is an excellent example of a functional React application with a simple yet significant feature, game history, and is ideal for those who want to explore the practical implementation of React hooks.

---
Please note that the game logic function `calculateWinner()` is outside of the components which checks each possible combination of positions for a win, keeping our components clean and single-purposed.
