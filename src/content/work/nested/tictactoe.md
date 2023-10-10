---
title: Unbeatable Ultimate TicTacToe AI
publishDate: 2023-05-15 00:00:00
img: /assets/miniature_tic.jpg
img_alt: Screen of the working AI
description: |
  In my third year, I programmed an AI in Python that could not be beaten in the unknown game of Ultimate TicTacToe 
tags:
  - Python
  - Mini-Max Algorithm
  - Alpha-Beta Pruning
---

## Rules of the game
The game of Ultimate TicTacToe is an unfamous game that derives from Tic Tac Toe. It is a Tic Tac Toe gameboard that has inside each of its case a game of Tic Tac Toe.


<img src="/public/assets/demo.jpg" alt="how the game works" width="100%">
As shown in the image, once you play in a case of a small board, the next player has to play in the board corresponding to the case you played in. if you play in the case 3, the next play has to play in the Tic Tac Toe numbered 3. 

## Working of the algorithm
The algorithm works with an **Alpha-Beta Pruning**, meaning that once you find the best utility possible, it stops running and returns the play with the best utility.
The algorithm works based of these concepts:
- Since we had to beat others classmates's algorithms, I based my algorithm on the fact that the adversary algorithm would play the best play.
- The algorithm does not play in a case that will offer direct victory to the opponent in the next tictactoe.
- To have the best results because speed was a factor, the algorithm will simulate only 5 next plays (depth = 5).

## Demonstration

<video controls width="100%" muted controlsList="nodownload">
  <source src="/assets/tictactoe_demo.mp4" type="video/mp4">
</video>
