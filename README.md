# MathsModel_PragathiKelkar
### ACM40960 - PROJECTS IN MATHS MODELLING 2022/23
### PRAGATHI KELKAR-22202401,           HANIMI GOLAMARI-22202328
# Single Deck Blackjack Simulation

This README includes an overview of the project, instructions for running the simulation, a discussion of the methods used, results validation, and comparisons of single- and multiplayer scenarios.


![Blackjack Logo](Blackjack logo.png)

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Simulation Details](#simulation-details)
- [Results](#results)
- [Contributing](#contributing)
- [Pending Features](#Pending-features)
- [License](#license)
- [Contact](#contact)

## Introduction

Blackjack is a card game in which players fight against a dealer to get as near to 21 as they can without going over.Each card has a specific value.Players are dealt two cards, and they can choose to "hit" and get more cards or "stand" with their current cards. The goal is to have a higher total than the dealer without exceeding 21. If a player's total goes over 21, they lose the round. The player with the closest total to 21 without going over wins.
Monte Carlo simulations use random sampling to generate a large number of scenarios or trials.

Here we attempt to simulate a blackjack game[simulate_game] multiple times with random input to calculate the Win/loss/tie probabilities[calculate_probability] for single/multiple player game using single deck of cards and validate the results using a actual real life dataset.



## Features
- One deck of cards is used to simulate blackjack games in this feature.
- Examine the likelihood of winning using various player strategies.Three strategies are used Here:
  1. agressive >17 continuous hit
  2. Basic <17 hit 
  3. Balanced between 14 to 18, randomly hit and stay

- We illustrate with an example,what the probability of winning/loosing is if a player takes another card.
- Simple-to-use R script for simulation execution.
- Implemented code for single player as well as multiplayer simulated for 10,000 times using monte carlo method with random inputs.
- We validated the results using a real dataset for multiplayers.


## Requirements
To run the simulation, you need:
- R programming language (version R-4.3.1 or later)
- Rstudio (version 3.3.0 or later )
- Basic understanding of Blackjack rules and strategies.
  
## Installation
1.Clone this repository to your local machine and run in R studio.

## Usage

Modify Parameters:

Inside the script, you'll find configurable parameters such as the number of simulation runs, players, and strategies.
Adjust these parameters according to your simulation scenario. For example:
num_simulations <- 100000
num_players <- 2
player_strategy <- "balanced"

#### Why the project is useful?
We can show how much chances are there for a player or the dealer to win the bet in a game.


#### Where users can get help with your project?
We have referred the following :
 1.Akkar, A., Cregan, S., Cassens, J., Vander-Pallen, M.A. and Mohd, T.K., 2022. Playing Blackjack Using Computer Vision. In Artificial Intelligence and Applications
Dong, H., Mao, J., Lin, T., Wang, C., Li, L., and Zhou, D., 2019. Neural logic machines. arXiv preprint arXiv:1904.11694.

2.Green, M.C., Khalifa, A., Charity, M., Bhaumik, D. and Togelius, J., 2022, July. Predicting Personas Using Mechanic Frequencies and Game State Traces. In 2022 IEEE
Congress on Evolutionary Computation (CEC) (pp. 1-8). IEEE.

3.Reinhardt, J., 2020. Competing in a complex hidden role game with information set monte carlo tree search. arXiv preprint arXiv:2005.07156.
Vidámi, M., Szilágyi, L. and Iclanzan, D., 2020. Real-Valued Card Counting Strategies for the Game of Blackjack. In Neural Information Processing: 27th International
Conference.
 
 4.ICONIP 2020, Bangkok, Thailand, November 23–27, 2020, Proceedings, Part II 27 (pp. 63-73). Springer International Publishing


## Simulation Details

Case 1: The above process should be implemented for multiplayer(6 players,1 dealer)
-a)Fix strategies to each player(eg:P1-basic,P2-aggressive etc) :
- compare win,loss,tie percentage for all players after 10,000 simulations.
-Also compare this percentages with single player with same strategy.
b)Strategies are assigned randomly to each of players : 
- After monte carlo(10k) simulations,find what is the win,loss and tie percentage.
-Analyse which player used which strategy most and predict what he will most likely use in future.
-Show the relationships between players(if any scatter plot or similar).

Case 2:- Analyse an actual dataset with multiple games,6 players,dealer and who wins.Validate if the Monte carlo simulation results are similar w.r.to each player's winning/lose/tie probabilities. -|- Check if there are any relationships or correlations between players.
- Analyse Which strategy is more likely to win.


Case 3:-Give one example of a blackjack multiplayer game simulation.
Where in once the 2 cards are distributed, the player can find out the probability of winning if he draws another card,or if he can win if he stays.Display the probabilities.
-Show which strategy must he  implement while playing,to increase chances of winning.
and show an output of winning probability for each player,
      if he hits extra one card(considering what other players have drawn)
      If he hits extra 2nd extra card.

-We Created different plots showing interrelationships wherever possible.And have written likeliihood and interpretation/inference we get from each plot.


## Results


## Contributing
You can suggest and give insights on how we can better the project or simulations.

## Pending Features



## License


## Contract
## Usage/Examples

```javascript
import Component from 'my-project'

function App() {
  return <Component />
}
```

