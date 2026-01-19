A Python project I developed aimed at creating an explainable chess AI, including scoring functions, move explanation functions, and integration with preexisting chess agents. I also created a genetic algorithm to generate weights for the chess agent's scoring functions.

How to run locally:
```
# Create a virtual environment and activate it.
python -m venv .venv
. .venv/bin/activate

pip install python-chess chess stockfish --upgrade

# Install Stockfish on Linux (Ubuntu)
# Or see https://github.com/official-stockfish/Stockfish/wiki/Download-and-usage
sudo apt install stockfish

# Find Stockfish location, usually `/usr/games/stockfish`.
which stockfish

# Use the result from `which stockfish` for `STOCKFISH_BIN` in the notebook.
```

```GRG_chessXAI_genetic.ipynb``` is used to run a genetic algorithm to generate weights used in the explanations. (I wouldn't run this unless you have a bunch of cores free and are prepared to wait a good long while.)

```GRG_chessXAI_player.ipynb``` is used to run the player and explain moves.

