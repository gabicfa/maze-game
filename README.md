# maze

This project implements a game in which the player from a starting point must guide a character controlled by the four arrow keys to an ending point of a maze. This maze is read from a file in a specific format and displayed via Swing.

In addition, this character competes with a computer-controlled second, whose artificial intelligence is based on a stack-based depth-first search. The idea behind this algorithm is simple: a pile is used as a “trail of bread crumbs”, indicating to the computer the path taken from the starting point. When it runs into a dead-end, unstacking represents a “step back” on that trail, which allows it to try other paths previously ignored.

When one of the two characters reaches the exit, the game ends by naming the winner. Note that the maze generator allows changing dimensions via the constants WIDTH and HEIGHT, so the program is prepared for mazes of arbitrary sizes. 