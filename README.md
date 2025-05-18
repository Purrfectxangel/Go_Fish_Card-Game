# Go_Fish_Card-Game
The final project for Stevens course EE551 is to implement a card game via Python and Objected Oriented Programming (OOP). I implemented a Go Fish card game. Needless to say, I had great fun making this game.

### 🐟 General Description of "Go Fish"
"Go Fish" is a simple card game where players try to collect matching sets of four cards of the same rank, also known as "books". The goal is to win the most "books" of cards. The game can be played by 2 or more players, up to 6 players.

🎨 __*Creative Touch*__: 
-  The deck and draw pile will be implemented via Numpy. The final score board to display player scores will be implemented via a Panda DataFrame.
-  Multiple Python data structures are utilized based on their functionalities and limitations to complete classes and functions for the game: list, dictionaries, Numpy array, Panda DataFrame.
-  I have the program taking in inputs from users to as an interactive feature as another creative touch. I also added input validation loops to make sure the user is entering the right and valid value.
-  A mechanism in the game initiation function to make sure there are only 6 players: I used a sys.exit() function with a customized message to terminate the program if the user enters a number over 6 as number of player and telling the user the reason for the termination.
-  Overall I have tried to do everything I personally can think of with Python to make the game fun and easy to use for the players so it feels more like a game instead of just an OOP programming class project. (I'm a huge fan of video games so I feel like it's sin if I don't try as much as I can to make a game feel more like a game.)

### 📜 "Go Fish" Game Rules:
1. Shuffle a standard deck of cards. If there are 2 or 3 people playing, deal 7 cards to each player. If there are 4 or more people playing, deal 5 cards to each player.
2. Players take turns asking another player for cards of a rank, e.g. ask "Do you have any Ace?"
3. If the player being asked has cards of the requested rank, then he or she must give all cards of this rank to the requester
4. If the player being asked have no cards of the requested rank, then it's "Go Fish" time: the requester will draw a card from the draw pile (aka the "Fish Pond").
5. During a turn, if a player failed to get cards from another player and also failed to find a card of their requested rank (a fish) from the draw pile (fish pond), then they cannot continue their turn. It will be the next player's turn in this case.
6. If any player collects a "book", a set of 4 cards of the same rank, this player should immediately lay the "book" down in front of them and remove them from the hand.
7. The game ends when some player run out of cards or when there is no more card in the draw pile. The player with the most number of "books" wins the game.

### 🚨 User Instructions:
1. Below all the game codes and game play demo towards the end of this Jupyter Notebook, I added cells that will initiate and play the "Go Fish" game based on number of people. Please select the cell with number of players you desire and input their names in each string in the string list and run the cell to start a game.
2. Should you want to initiate and run your own game yourself:
    -  Initiate a new game instance of "go_fish_game" class:
          - "Go Fish" can have up to 6 players. So when you initiate a new game instance, please pass a number(int) of less than 6 players as argument. Or the program will terminate with a message customized by me telling you why.
    - Then use the play() function of the game instance you initiated to start playing the game:
      -  Please pass the names of the players as a list of strings as argument when you use the play() function. Make sure the number of player names in the list is the same as the number of players you entered when you initiated the game.
3. In the game, you will be prompted when it is your turn and will be asked on which other player you would like to request card from and which card rank you are asking for:
    - For Your Input on the Name of Your Opponent: please make sure to enter the player name string from the list of players you entered when you start the play session. If you enter incorrectly, you will be asked to re-enter.
    - For Your Input on Rank of the Card You Want: please enter the rank of card as per the string of rank list of "Ace", "2", "3", "4", "5", "6", "7", "8", "9", "10", "Jack", "Queen", "King". If you enter incorrectly, you will be asked to re-enter.
4. Through out the game, you will be informed of all the necessary information you need like what cards you got from another user or what card you caught as a fish or what is your current score or which rank of book of 4 cards you just accumulated when you manage to accumulate a book of 4 cards of the same rank. 
5. Enjoy!
