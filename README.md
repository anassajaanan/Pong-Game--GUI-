# Ping Pong Game

<p align="center">
  <img src="https://media.discordapp.net/attachments/1055044134303453226/1055779731095703653/Screenshot_65.png?width=924&height=489" width="300" alt="Ping Pong game animation">
</p>

This project is an implementation of the classic ping pong or table tennis game using the Python Turtle library. The Turtle library is a built-in library in Python that is used to create simple graphics and visualizations.

The game involves two players who use paddles to hit a ball back and forth across a vertical line in the middle of the screen. The goal of the game is to score points by hitting the ball past the opponent's paddle and into their side of the screen.

## How to Run the Game

To run the game, you will need to have Python 3 installed on your computer. You can then download the game files and run the `game.py` file using the following command:

```bash
python game.py
```

## Game Controls
The game can be played using the following keyboard controls:

- Player 1 (left paddle):
   - Up arrow key: move paddle up
   - Down arrow key: move paddle down
- Player 2 (right paddle):
   - W key: move paddle up
   - S key: move paddle down
   
## Game Classes

The game consists of three main classes:

### Ball

The `Ball` class is a subclass of the `Turtle` class and is used to create and animate the ball in the game. It has the following attributes and methods:

- `__init__`: initializes the ball with a specific shape, color, size, and starting position on the screen. It also sets the ball's movement direction and speed. The ball's movement direction is determined by the values of `self.dx` and `self.dy`, which are set to either 1 or -1 in the `__init__` method. The ball's movement speed is determined by the value of `self.speed`, which is set to 25 in the `__init__` method.
- `move_ball`: updates the ball's position based on its current position and its movement direction and speed. The ball's position is updated by setting its `x` and `y` coordinates using the `setx` and `sety` methods. The ball's movement direction is also checked to see if it has hit the top or bottom edge of the screen, in which case it is reversed.

### Line

The `Line` class is a subclass of the `Turtle` class and is used to create the vertical line in the middle of the screen. It has the following attributes and methods:

- `__init__`: initializes the line with a specific color, size, and position on the screen. It also creates a series of smaller squares that make up the line. The squares are spaced apart from each other and are positioned vertically on the screen.
- `hideturtle`: hides the turtle cursor.

### Paddle

The `Paddle` class is used to create the paddles that the players use to hit the ball. It has the following attributes and methods:

- `__init__`: creates two lists of `Turtle` objects, one for the right paddle and one for the left paddle. It also creates the right and left paddles by calling the `creat_paddle` method.
- `creat_paddle`: creates a paddle by creating a series of small squares that

## Gameplay
   During gameplay, the ball will move back and forth across the screen, bouncing off the top and bottom edges and the paddles. The players can use the keyboard controls to move their paddles up and down in order to hit the ball back to the opponent. If a player misses the ball or hits it out of bounds, the opponent scores a point. The game continues
