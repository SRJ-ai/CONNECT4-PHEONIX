# connect4
It's a connect-4 game,2-player game,by connecting colours horizontally,vertically(or)diagonally.
About html:
This is an HTML file that represents the user interface of the Connect 4 game. 
It uses the <html>, <head>, <meta>, <title>, <link>, <body>, <h1>, <h2>, <div>, <ul>, and <p> elements to create the layout of the game.

The <head> element contains the <meta> element that sets the character encoding and the <link> element that links the external CSS file that styles the game.

The <body> element contains all the elements that make up the game, such as the title, the message displaying whose turn it is, and the game board. 
The background image is set to cover the entire body and center it by using the background-image, background-size, background-position, and background-repeat properties.

The <h1> element displays the title of the game, and the <h2> element displays the message about whose turn it is.

The <div> element with the class "board" contains all the elements that make up the game board. 
The "board" class is styled with CSS to create the grid layout of the game board.

The <ul> element with the class "column" is used to create the columns of the game board. 
Each <ul> element has an id that corresponds to the column number, and it contains several <p> elements that represent the cells of the game board.
Each <p> element has an id that corresponds to the row and column numbers.

The script tag at the bottom of the file links to the external JavaScript file that controls the logic of the game.

Overall, this HTML file creates the structure and layout of the Connect 4 game. 
It uses CSS and JavaScript to control the appearance and behavior of the elements on the page.

ABOUT CSS:

This is a CSS code that styles the Connect 4 game. It sets the font-size, margins, padding, and the layout of the elements on the page. 
The code uses CSS Grid Layout to create a grid system and center the elements on the page.
The body element is set to display: grid and place-items: center, which centers all the elements inside it horizontally and vertically. 
The .board class is also set to display: grid and grid-template-columns: repeat(7,1fr), which creates a grid with 7 columns.
Each of them taking up 1 fraction of the available space.
The border, width, and background-color properties are used to style the board and give it a border and a specific background color.
The ul element is set to display: grid and place-items: center, which centers the items inside it horizontally and vertically.
The p element inside it is given specific width, height, border, and background color properties.
The media queries at the bottom of the code are used to change the layout and styles of the elements based on the screen size.
For example, if the screen width is less than 700px, the width of the board and the chip size are reduced.
This CSS code is used to make the Connect 4 game visually appealing and responsive to different screen sizes.


ABOUT JS:
This is a JavaScript code that implements a Connect 4 game.
The game board is represented by a table in an HTML file, and the JavaScript code is used to determine the winner of the game by checking the background color of the table cells. 
The check() function checks if the background color of four consecutive cells in a row, column, or diagonal is the same as the specified player's color, which is either "red" or "yellow".
If the function finds such a sequence of cells. I
t alerts the winner and reloads the page. The document.querySelectorAll(".column") selects all elements with the class "column" and adds a click event listener to each of them, 
so that when the user clicks on a column, the corresponding cell at the bottom of that column will be colored with the current player's color, and the turn will switch to the other player.
Additionally, the code also uses variables val_c1 through val_c7 to keep track of the number of chips already placed in each column, 
so that the new chip is placed at the bottom of the column. 
It also uses the turn variable to alternate between players and the whosturn element to display the current player's turn.
It's also worth noting that the code uses setTimeout function which delays the execution of check function by 200ms which allows the chip to be placed before checking the winner.


