# Tic-Tac-Toe

Tic Tac Toe
Introduction
In this article, we will explore a code snippet for creating a Tic Tac Toe game using HTML, CSS, and JavaScript. We will break down the code and explain its structure and functionality.

Key Concepts
The key concepts involved in this code are:

HTML structure: The HTML code defines the structure of the game board and the buttons used for gameplay.
CSS styling: The CSS code provides the visual styling for the game board, buttons, and popup messages.
JavaScript logic: The JavaScript code handles the game logic, including checking for wins, draws, and enabling/disabling buttons.
Code Structure
The code is structured into three main sections: HTML, CSS, and JavaScript. Let's take a closer look at each section.

HTML
The HTML section defines the structure of the game board and includes the necessary elements for gameplay. It consists of a <div> with the class "wrapper" that contains a <div> with the class "container" for the game buttons. The "Restart" button is placed outside the container. Additionally, there is a hidden popup <div> for displaying messages.

CSS
The CSS section provides the visual styling for the game. It includes styles for the overall layout, background, button appearance, and popup messages. The styles are applied using class selectors and element selectors.

JavaScript
The JavaScript section contains the logic for the Tic Tac Toe game. It starts by selecting the necessary elements from the HTML using query selectors and assigning them to variables. It also defines a winning pattern array that represents all possible winning combinations on the game board.

The code then defines several functions:

disableButtons(): Disables all game buttons and shows the popup message.
enableButtons(): Enables all game buttons, clears their text, and hides the popup message.
winFunction(letter): Disables buttons, displays a winning message based on the winning letter ('X' or 'O').
drawFunction(): Disables buttons and displays a draw message.
Event listeners for the "New Game" and "Restart" buttons that call the enableButtons() function and reset the game.
Finally, the code adds event listeners to each game button. When a button is clicked, it checks if it's the X player's turn or the O player's turn. It updates the button text accordingly, disables the button, increments the move count, and checks for a win or draw condition using the winChecker() function.

Code Examples
Here are some code examples from the provided snippet:

HTML
language-html
<div class="wrapper">
    <div class="container">
        <button class="button-option"></button>
        <!-- More buttons... -->
    </div>
    <button id="restart">Restart</button>
</div>
<div class="popup hide">
    <p id="message">Lets Play</p>
    <button id="new-game">New Game</button>
</div>
CSS
language-css
 Copy code
/* CSS styles for the game board and buttons */
.container {
    /* Styles... */
}

.button-option {
    /* Styles... */
}

/* CSS styles for the popup message */
.popup {
    /* Styles... */
}
JavaScript
language-javascript
 Copy code
// JavaScript logic for the Tic Tac Toe game
let btnRef = document.querySelectorAll(".button-option");
let popupRef = document.querySelector(".popup");
let newgameBtn = document.getElementById("new-game");
let restartBtn = document.getElementById("restart");
let msgRef = document.getElementById("message");

// Winning pattern array
let winningPattern = [
    [0, 1, 2],
    [0, 3, 6],
    // More winning patterns...
];

// Functions for game logic
const disableButtons = () => {
    // Code...
};

const enableButtons = () => {
    // Code...
};

const winFunction = (letter) => {
    // Code...
};

const drawFunction = () => {
    // Code...
};

// Event listeners for "New Game" and "Restart" buttons
newgameBtn.addEventListener("click", () => {
    // Code...
});

restartBtn.addEventListener("click", () => {
    // Code...
});

// Function to check for wins
const winChecker = () => {
    // Code...
};

// Event listeners for game buttons
btnRef.forEach((element) => {
    element.addEventListener("click", () => {
        // Code...
    });
});

// Function to enable buttons on page load
window.onload = enableButtons;
Conclusion
In this article, we explored a code snippet for creating a Tic Tac Toe game using HTML, CSS, and JavaScript. We discussed the code structure, key concepts, and provided code examples for each section. By understanding this code, you can create your own interactive Tic Tac Toe game and enhance your web development skills. Happy coding!

Please help us by rating this answer:Tic-Tac-Toe is a classic game that has been enjoyed by individuals of all ages across generations. This guide will serve as a tutorial on how to create your own Tic-Tac-Toe game using HTML, CSS, and JavaScript. The guide will include an explanation of the code structure, key concepts, and will provide code examples for each section.

Through understanding the code, you will be able to create your own interactive Tic-Tac-Toe game and expand your web development skills. The guide will also provide a deeper understanding of the game's logic and help you develop a strong foundation in web development. By following the steps outlined in this tutorial, you will learn how to create a fully functional Tic-Tac-Toe game that you can share with friends and family or use as a personal project.
