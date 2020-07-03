# dice-a-game

SEI-23 Project 1

Game is hosted here: https://jia-hern.github.io/dice-a-game/

Project 1 Objectives
Create basic Game with HTML, JS and CSS

Game flow:
1. When both players are ready to start, someone clicks New game
1. Players would randomize the attack(atk) and health(hp) of their teddy bears by clicking on the Roll dice button
1. The left player(blue) would go roll the dice first, after which the right player(red) rolls the dice 
1. After all the attack and health are populated for all teddy bears, one player can click showdown
1. The player with more teddies left wins the game

May the odds ever be in your favor~

How does the game work:
DOM manipulation is used to create divisions which each contain a teddy bear image, attack and health. An unique ID is tagged to each feature.

An event listener is then added to the roll dice button, which updates the attack and health of the teddy bear based on the turn.

A conditional statement is then used to look for the turn where all teddy bears have their attack and health populated.

When this conditional statement is fulfilled, the visibility of the roll dice button is set to hidden while the showdown button is set to visible

Pressing the showdown button then allows the teddy bears on each row to duel each other. 

The duel works by subtracting the health based on the opposing teddy's attack until either side reaches zero.

The duel then stops for that row and the teddy image of that respective teddy is replaced with an angel teddy bear

An array is used to store the status of the teddy bears with alive being 1 and dead being 0.

The total number of teddy bears alive for each side is then computed based on the sum of each sides's array.

When all duels have finished, the win condition is determined based on which player has more teddies alive.
