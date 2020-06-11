# ActorCritic-Model

### Environment Description
The inverted pendulum swingup problem is a classic problem in the control literature. In this version of the problem, the pendulum starts in a random position, and the goal is to swing it up so it stays upright.

Action Space : 1

Observation Space : 3

Seed : 2

### Description
This is an Actor Critic model trying to solve the OpenAI gym's pendulum-v0. The repository contains the Actor Critic Networks trained weights. The implementation also adds a Ornsetein-Uhlenbeck noise to the action space.Adding noise to the parameters of a neural nwtwork can imporove its performance(https://openai.com/blog/better-exploration-with-parameter-noise/). Also we have included a replay buffer to include experience replay.

### Actor & Critic Network Parameters
BUFFER_SIZE = int(1e5)  # replay buffer size

BATCH_SIZE = 128        # minibatch size

GAMMA = 0.99            # discount factor

TAU = 1e-3              # for soft update of target parameters

LR_ACTOR = 1e-4         # learning rate of the actor 

LR_CRITIC = 1e-3        # learning rate of the critic

WEIGHT_DECAY = 0        # L2 weight decay





