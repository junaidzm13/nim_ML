# nim_ML

### Designed, developed and implemented an AI that teaches itself to play Nim through reinforcement learning.

## How to run?
  - In the repository, run **python play.py**
  
## Background
Recall that in the game Nim, we begin with some number of piles, each with some number of objects. Players take turns: on a player’s turn, the player removes any non-negative number of objects from any one non-empty pile. Whoever removes the last object loses.

There's some simple strategy you might imagine for this game: if there's only one pile and three objects left in it, and it's your turn, your best bet is to remove two of those objects, leaving your opponent with the third and final object to remove. But if there are more piles, the strategy gets considerably more complicated. In this problem, we have built an AI to learn the strategy for this game through reinforcement learning. By playing against itself repeatedly and learning from experience, eventually AI will learn which actions to take and which actions to avoid.

In particular, we have used Q-learning for this project. Recall that in Q-learning, we give try to provide a reward value (a number) for every (state, action) pair. An action that loses the game will have a reward of -1, an action that results in the other player losing the game will have a reward of 1, and an action that results in the game continuing has an immediate reward of 0, but will also have some future reward.

For more information regarding the game pleas visit [Wikipedia](https://en.wikipedia.org/wiki/Nim)

## Acknowledgement
  - Special thanks to CS50AI 2020: Introduction to Artificial Intelligence with Python course's managment, lecturers and tutors.
