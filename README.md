# Permutation-Puzzles-Kaggle-
# Project Description
This project is designed to produce entries for the kaggle competition "Santa 2023 - The Polytope Permutation Puzzle", which can be found at https://www.kaggle.com/competitions/santa-2023/overview.
Essentially, the goal is to find solutions to puzzles similar to rubik's cubes while using as few moves as possible. A file with (highly inefficient) solutions is given, so my goal is simply to improve on these solutions.

# Method
In order to solve this problem, I used Sympy's permutation features. I started by writing a function that produces a dictionary containing all permutations that can be achieved within a fixed number of moves,
and corresponds them to the sequence of moves giving that permutation. I then wrote a function that searches through a given solution to a puzzle, and checks for any possible shortcuts, i.e. a sequence of 
moves in the given solution that could be achieved by a shorter sequence of moves. It then replaces that sequence with the more efficient sequence. Finally, by running this procedure many times, the lengths of
the solutions can be dramatically decreased. In the near future, I will add a document to this repository with a more detailed account of how this procedure works as well as some of the improvements that I made along the way.

# Results
The competition ends at the end of January, so I will be running this procedure many times before then, for now this procedure has managed to eliminate 30,000 unnecessary moves from the given solutions, but with some improvements 
to the efficiency of the functions, and more timem to run the program, I believe that I will see dramatically more moves removed by the end of the competition.

# Skills demonstrated
Sympy
Dynamic Programming
Optimization
Problem Solving
