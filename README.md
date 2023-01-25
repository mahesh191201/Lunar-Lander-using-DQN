
# Lunar Lander using DQN

The main goal of this project is to land the spacecraft between two flags in
a stable manner. The landing pad is always situated at coordinates (0, 0). The reward
for moving from the top of the simulation screen to the landing
site ranges from 100 to 140. If the lander moves away from
the landing site, it loses reward points. The episode finishes
when the lander crashes or comes to rest, for which it may
receive either -100 or 100 points.

State Space

There are eight state variables associated with the state
space for the LunarLander-v2 environment.

• x: horizontal coordinate of the lander

• y: vertical coordinate of the lander

• vx: horizontal velocity of the lander

• vy: vertical velocity of the lander

• θ: orientation in space

• vθ: angular velocity

• Left leg touches the ground (Boolean)

• Right leg touches the ground (Boolean)

Action Space

Four actions are possible do
nothing, fire left orientation engine, fire main engine, and fire
right orientation engine. If the left and right engines are fired,
these actions introduce torque to the lander which causes it to
rotate. This rotation makes stabilizing the lander difficult.

Q-Learning

A reward or penalty is expected for actions taken at every
episode. If the actions that yield the maximum reward are
known in advance, the agent has the ability to choose such
actions to perform. It will perform a sequence of actions that
eventually generate the highest reward yield. The total reward
is also known as the Q-value and can be written as

Q(s, a) = r(s, a) + γmax
a
Q(s
0
, a)


## Screenshots


![App Screenshot](https://github.com/mahesh191201/Lunar-Lander-using-DQN/blob/master/demo/lunarlanderpost-2.png?raw=true)



![App Screenshot](https://github.com/mahesh191201/Lunar-Lander-using-DQN/blob/master/demo/graph.jpg?raw=true)



https://user-images.githubusercontent.com/85864151/214515472-be068ee9-0405-4081-a619-9c10074c241a.mp4



