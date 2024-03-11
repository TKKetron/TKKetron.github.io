---
title: "Snake and Minesweeper AI"
excerpt: "An ai program used to solve the games of Snake and Minesweeper"
collection: portfolio
---

I had learned about AI and making neural networks in my senior year of highschool. There I decided to learn how to make a simple neural network following the deep learning AI model. AI that learned how to do something from nothing was always very interesting to me. since then I have made an AI class that creates a neural network and learns on its own. It follows a simple mutation and fitness algorithm in order to train the network over many generations.

My first use for this was a simple snake game. Snake has always been a very interesting game to me, because it follows a very simple algorithm. The ai I made took a while to learn how to actually play the game. The way the AI works is I give it an input layer, then some backend processing happens in the hidden layer, and finally it gives me an output layer.

At first I defined the input layer as all the information I could give it. I defined all the values I could and fed it into the network. with the output layer being thee values, left right or no change. After many generation andd many tests with different hidden layers no change was occurring so I decided to simplify the network. After changing the network to a simple input layer this time only giving values, distance from head to wall, distance from head to food, and distance from head to tail, it started to perform much better, but still was less than ideal. My last test was the same, but I added angle to food. Finally this allowed the snake to make better decisions and learn at a descent rate.

This was the simple UI i threw together in order to train the AI. It has a simple learn button, which taught 1 generation. I added a checkbox so that it would learn on repeat. and finally a Kill button to kill the current snake being displayed so it would update to the latest generation.

[Snake AI](/images/AI/snake%20ai.png)

Check out the code [HERE](https://github.com/TKKetron/Snake-AI)

During my senior year of college I revisited the project and worked on a minesweeper AI. Much like the snake AI I used the same class and operated the same way. I created an input layer that was the size of the minefield and an output layer the same size. Whatever value the AI outputted is the value that was clicked.

[Simple Minesweeper](/images/AI/simple%20minesweeper.png)

The challenge with this was the time it took to train and aggregate data. The start was similar to that of the snake AI. I had to create minesweeper from scratch in order to read the field and output the value I wanted to be clicked via code. This was the easy part though. Having the AI actually learn at a reasonable rate takes a long time with a lot of testing.

[Learning AI](/images/AI/minesweeper%20learning.png)

This process is simple, just time consuming. There are known better ways to do this, especially with pre made libraries like TensorFlow in python. I have used those before in various classes, but I still enjoy the process of making this all myself. I have learned a lot form this project and will continue to make AI in the future for fun. Next I believe I will try to make an AI with the NEAT model.

check out the minesweeper AI code [HERE](https://github.com/TKKetron/MineSweeper-AI).