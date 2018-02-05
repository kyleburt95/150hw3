Assignment 3: Gomoku with Monte Carlo Tree Search
=========

Your task is to implement the MCTS method for playing Gomoku. The base game engine is from [here](https://github.com/HackerSir/PygameTutorials/tree/master/Lesson04/Gomoku). 

Due date
-----
Feb-24 11:59pm Pacific Time. Extra credits for earlier submission (see below). 

The Game
-----
Gomoku is a popular game played on the Go board, following much simpler rules. 

- There are two players, one placing black pieces and the other white pieces, at the grid intersections of the board. 
- The two players take turns to place one piece each time. Pieces are never moved or removed from the board. 
- The players' goal is to have five pieces of their own color to form an unbroken line horizontally (`examples/ex1.png`), vertically (`examples/ex2.png`), or diagonally (`examples/ex3.png`). Of course, these are unlikely realistic games between reasonable players. A real game is more like `examples/ex4.png` (black is still very lame in the end).  
- The game engine starts with human against a random-play agent. Click any grid intersections and see what the computer does. Press enter to see a random game between two random-play agents (also press enter to pause autoplay and switch back to human vs random). Press 'm' to switch to manually playing both sides.  

Grading
-----
- Regular Commits (1 points)

You should at least one nontrivial commit by Feb-17 11:59pm. 

- Documentation (1 points)

Comment your code generously. 

- Functionality (10 points)

The MCTS agent should use the standard Monte Carlo Tree Search methods, and consistently beat the random-play agent. 

In the starter code, the automated game (press Enter) is played between two random-play agents. You need to change one of them to an MCTS agent (See the `#TODO` line in the `Board.autoplay` function). 

Read the code for the random-play agent in `randplay.py` carefully. It is more verbose than needed for a random player, just to provide hints for functions that you may need in the MCTS code. In particular, you may want to (not required) implement the random rollout function in the `Randplay` class which can be used in the MCTS class. 

Again, the template in MCTS is just a suggestion. Feel free to change the paramters used in the functions. 

Extra credits (up to 4 points)
------
- 1 extra point for showing on the board the winning line of five pieces (for instance, draw a line through them, or circle each of them). 
- If your last commit is pushed by Feb-17 11:59pm, with no significant bug, then you will earn 3 extra points. 
- If your last major commit is pushed by Feb-17 11:59pm, with also one minor commit after that (definition of a minor commit is less than 5 lines of changes in total), and with no significant bug, you can earn 2 extra points. 

Note
------
- Make sure to start early. It requires more work than Assignment 2. 
- At the deadline, Github will automatically save the last commit as your submission. Make sure to commit your full solutions before that, and also your name and PID in the README.md file.  
