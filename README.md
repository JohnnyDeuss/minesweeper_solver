# Minesweeper solver
A minesweeper solver that uses a number of techniques, such as constraint programming and math, to find the exact
probability that squares contain a mine. It optimally solves a single state, but picking the right square relies on more
than knowing the exact probabilities, as each move can make subsequent moves easier by, for example, being more likely
to constrain the value of already constrained squares. The method for picking which square to open is called the policy
and finding a near-optimal policy requires machine learning. Some simple policies are given in `/solver/policies`.

![An example of the solver doing its thing.](/examples/example.gif)

## Installation
The solver can be installed directly from GitHub
using the following command:

`pip3 install git+ssh://git@github.com/JohnnyDeuss/minesweeper_solver#egg=minesweeper-solver`

To run the GUI example, the [minesweeper GUI](https://github.com/JohnnyDeuss/minesweeper) must be installed, which can
either be installed separately or can be automatically installed by adding the GUI option to the above command:

`pip3 install git+ssh://git@github.com/JohnnyDeuss/minesweeper_solver#egg=minesweeper-solver[GUI]`

## Usage
A couple of examples of the solver being used to solve minesweeper games are given in the `/examples` directory.
