# Banana Navigation

## Learning Algorithm
 
* This project uses Deep Q Learning with state size of 37. Below is the sequential architecture of the Deep Q Learning model.

```
Tanh(Fully Connected Layer 1 with 37 as state size and 96 as hidden node size)
```
```
Tanh(Fully Connected Layer 2 with hidden input of 96 and 96 as hidden node size)
```
```
Tanh(Fully Connected Layer 3 with hidden input of 96 and 96 as hidden node size)
```
```
Output layer with hidden input of 96 and output of actions
```

The default hidden node size of 64 was not learning quickly. So i began to increase the size and it did wonders with 96 as the final size.
Tanh activation function was performing better than Relu and sigmoid. The advantage is that the negative inputs will be mapped strongly negative and the zero inputs will be mapped near zero in the tanh graph.
The other hyper parameters were:

```
BUFFER_SIZE = int(1e5)  - replay buffer size
BATCH_SIZE = 64 - minibatch size
GAMMA = 0.99  - discount factor
TAU = 1e-3  - for soft update of target parameters
LR = 5e-4  - learning rate
UPDATE_EVERY = 5  - how often to update the network
```

## Plot of Rewards

<img src="/graph.png" width=500 px />

<img src="/Avg score.png" width=700 px/>


## Ideas for Future Work

* Design a convolutional neural network as the DQN architecture to solve this environment 
