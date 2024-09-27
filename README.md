# chess-engine
Core Information:
  Start Date: 9/27/2024
  By: Jamieson Mansker

Lots of more research is still going to be required...

Objective:
  Create a chess engine in C++.
  
  MinMax algorithm used, coupled with an evaluation algorithm that uses a compilation of 2D arrays of weights corresponding to each piece and its general location on the board to catorgorize certain moves as "better" than other moves. This algorithm particularly will be optimized hopefully to limit search time for moves that can be written out early on and removed from the tree of possible moves. Additionally, these arrays of weights would change as pieces are removed off the board, and the game progresses. 
  
  For instance, king development in the end game once pieces are off the board is a much smarter strategy than rushing your king out into the center early on in the game.
  So we are going to update these weights for the arrays after each move. 

  Another more complicated example, might be that generally, if your opponent only has a light squared bishop, then it would make sense to position your pawns on light colored squares, preventing their bishop from moving as freely. So the pawns boards might be updated appropriatly following the removal of certain pieces.

  Of course, after the program calculates a certain move and evaluates that instance of worth, then it will continue checking subsequent moves, which is exponential. Once a move in the tree of possible moves (a line) is shown to not be as efficient as another, we can discard this particular line and continue on that other line.

  Another way to improve this algorithm is to keep track of the second best move for the last move that you made, and start with that the second time. This would more likely lead to finding the best line quicker unless the opponent moved a piece that made this move worth less.
  
  I want to improve this engine after finishing it initially as well. A goal of mine would be to achieve roughly 2000 elo, which I will test by publishing the both through Lichess.

Research:
  I've been wanting to do this project for a while now, and finally at this point in my schooling at WSU, I feel that I have the ability and confidence that I can create this chess engine and reach my goal of 2000 elo. What initially made me interested in this project was a youtube video (https://www.youtube.com/watch?v=U4ogK0MIzqk&t) by Sebastion Lague, and his second video on the same program (https://www.youtube.com/watch?v=_vqlIPDR2TU).

  There are a lot of parts in this project that I know only the abstract parts of as of now or know near nothing as to how I'll solve them. So future research will be added here.



  
