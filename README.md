# ada-2019-project

**Presentation of the dataset**

The dataset we will work on is a collection of 20000 games of chess from users on the website lichess.org. Lichess is one of the most used website for playing chess online and 
is therefore a good source of data if one want to study in depth chess.
This set contains several informations about the game (set of moves, opening, starting and ending time, the winner...) and about the players (their ID, their rankings...).
It is important to note all moves are given in Standard Chess Notation, thus making it easy to follow each game turn by turn. In this simple system, each move is given by
the initial of the piece and the square it is being moved (ex: Qe4 means the Queen has been moved to the square e4). This notation is explained in detail at http://cfajohnson.com/chess/SAN/ .
In a similar way, the opening is also codified with the ECO system (https://www.365chess.com/eco.php) thus making it easier to analyze and (possibly) find patterns.
Note that a larger dataset (with more than 3 million games) is available: https://chess-research-project.readthedocs.io/en/latest/ . We will decide later if we need to use it depending on the results obtained and our ressources. 

**Research question**

Is it possible to determine the outcome of a game following its status turn by turn? How many turns are needed to get accurate results?

The idea is to engineer different features from the set of moves to train different classification algorithms and determine the outcome of the game. Of course we expect that in the first turns it won't be possible to be accurante but maybe after having spent a few turns in the middle game, the predictions start to match the actual outcome. Some features we could extract from the set of moves are the number of pieces each player has killed/lost, the control of the board (ie the proportion of squares a player is threatening with his pieces), which pieces are still alive. We would combine these "internal" features with "external" ones such as the ratings of the two player (and the difference between the two), the number of turns, the opening move.

**Evolution of the state of the game**

To be able to extract some features from the set of moves, we would need to study the evolution of the state of the game after each turn. This means we have to keep track of the board state (64 squares) and the 32 pieces and update both after each move. Note this would also be used to visualise a given game turn by turn.

**Milestones**

  - 15/11: design a way to keep track of the state of the game (in an efficient way)
  - 22/11: extract features and train the algorithm
  - 29/11: continue to train the algorithm, get a sense of which features are the more relevant
