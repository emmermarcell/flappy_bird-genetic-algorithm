# flappy_bird-genetic-algorithm

The code teached a genetic algorith model to play Flappy Bird.

The original implementation of the game in pygame is from 

https://www.codewithharry.com/](https://www.codewithharry.com/videos/python-tutorials-for-absolute-beginners-122/)https://www.codewithharry.com/videos/python-tutorials-for-absolute-beginners-122/

The inputs of the model has 4 inputs and 1 output and 1 hidden layer with a single neuron and a sigmoid activation function. The inputs are the following:

```bash
X[0] = upperPipes[upcoming_pipe]['x']-playerx-GAME_SPRITES['player'].get_width()    # The horizontal distance of the closest pipe
X[1] = upperPipes[upcoming_pipe]['y']-SCREENHEIGHT/6-playery                        # The vertical distance of the closest pipe
X[2] = playery                                                                      # The vertical position of the player
X[3] = playerVelY                                                                   # The players vertical velocity

