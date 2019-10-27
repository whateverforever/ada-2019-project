# ada-2019-project

**Presentation of the dataset**

The dataset we will work on is a collection of 20000 games of chess from users on the website lichess.org. Lichess is one of the most used website for playing chess online and 
is therefore a good source of data if one want to study in depth chess.
This set contains several informations about the game (set of moves, opening, starting and ending time...) and about the players (their ID, their rankings, the winner...).
It is important to note all moves are given in Standard Chess Notation, thus making it easy to follow each game turn by turn. In this simple system, each move is given by
the initial of the piece and the square it is being moved (ex: Qe4 means the Queen has been moved to the square e4). This notation is explained in detail at http://cfajohnson.com/chess/SAN/ .
In a similar way, the opening is also codified with the ECO system (https://www.365chess.com/eco.php) thus making it easier to analyze and (possibly) find patterns.

**Some ideas of analysis**

- What are the best openings?
- Is there a correlation between the ranking of the players and the way they play (opening used, number of turns...)?
- What is the survivability rate of each piece (i.e. the chance a given piece has to still be on the board at the end of the game)?
