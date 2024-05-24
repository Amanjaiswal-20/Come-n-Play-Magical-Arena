# Magical Arena

## Run

To run the program, run `npm start`.  
To run unit tests, run `npm test`.  

## Modelling

2 classes have been designed.

1. `Player` class represents a player with health, strength and attack stats.  
A player can attack other players using the attack_player() method.  
A player can roll the dice by calling the roll() method. 

2. `Arena` class contains a group of players (an `array` of `Player` objects).  
An arena can "host" a match between 2 players in the player list by calling the fight() method, and passing the respective indices of the players.

A few validation functions are added so that the program does not enter an infinite loop. 

Dummy data has been added into `data.json` at the root of the project which can be parsed to create an `Array` of `Player` objects. 

# Game Rules
Players take turns attacking and defending.
Each player rolls a six-sided die for their attack and defense.
Damage is calculated based on the attack value, die roll, and opponent's defense.
The game ends when one player's health reaches 0.

## Sample Gameplay
Enter Player 1 name: Alice
Enter Player 1 health: 50

Enter Player 2 name: Bob
Enter Player 2 health: 50

...

Player 1: Alice - Health: 30
Player 2: Bob - Health: 20
---------------

...

Player 1: Alice - Health: 0
Player 2: Bob - Health: 10
---------------

Bob wins!

##  For testing, functionality tests and negative tests are added, using the `assert` module.
Project includes the following commits:
# Initial Commit:
 Basic project setup, including directory structure and initial Java classes.
# Implementation of Player Class: 
  Added the Player class with attributes and methods to represent a player in the game.
# Implementation of MagicalArena Class:
  Added the MagicalArena class responsible for managing the battle between players.
# Implementation of Main Class: 
  Added the Main class as the entry point for the game, handling user input and gameplay logic.
# Unit Testing Setup: 
  Configured JUnit testing framework and added initial test cases for Player and MagicalArena classes.
# Refactoring and Bug Fixes: 
   Refactored code for better readability and fixed bugs identified during testing.
# Final Testing and Documentation: 
   Completed testing for all classes and methods, added comprehensive documentation for the project.
