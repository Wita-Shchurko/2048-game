# 2048 game

[PLAY 🎮](https://Wita-Shchurko.github.io/2048-game/)

This is my implementation of the popular game "2048" using HTML, CSS, and JavaScript. Here's an overview of how the game works:

* HTML and CSS:
  * The game layout consists of a grid (game_field) where tiles are placed.
  * Tiles have values (2 or 4) and are styled with background and text color based on their values.
  * There are messages for different game states (e.g., start, win, lose) that can be displayed or hidden.

* JavaScript:
  * Classes:
    * Cell: Represents a cell in the game grid. It manages linked tiles, merging tiles, and checking conditions for movement.
    * Grid: Represents the game grid, consisting of cells. It groups cells by columns and rows for movement calculations.
    * Tile: Represents a tile with a value. It handles styling, animation, and removal from the DOM.

  * Initialization:
    * The game initializes with a 4x4 grid and sets up event listeners for keyboard input.
    * Tiles are randomly placed in two empty cells at the beginning of the game.

  * Game Logic:
    * Moving Tiles:
      * Tiles can be moved in four directions: up, down, left, and right.
      * Movement is implemented by sliding tiles in the specified direction.
      * Tiles slide until they reach the edge or collide with another tile.
      * Tiles with the same value merge into one, doubling the value.
      * The game checks for possible moves and displays a win or lose message accordingly.

    * Score:
      * The game keeps track of the player's score, which increases when tiles are merged.

    * Restart:
      * The game can be restarted by clicking the "RESTART" button.
      * The score is reset, and new tiles are randomly placed on the grid.

    * Win/Lose Conditions:
      * If a tile with a value of 2048 is created, a win message is displayed.
      * If there are no more possible moves, a lose message is displayed.


This code creates a functional and interactive implementation of the 2048 game, allowing players to make moves, merge tiles, earn points, and ultimately win or lose the game based on the game's rules.
