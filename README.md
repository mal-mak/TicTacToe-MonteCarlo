# Installation & Usage

1. Install [uv](https://docs.astral.sh/uv/getting-started/installation/)

2. Run the following commands:
	```bash
	git clone https://github.com/mal-mak/TicTacToe-MonteCarlo.git
	cd TicTacToe-MonteCarlo
	uv python install 3.12
	uv sync
	``` 

3. Open the [notebook](ttt.ipynb) and select **.venv (Python 3.12.*)** as the kernel.

4. All done, you can run the notebook.uv 

# Results

As you can see in the [Simulation Results](plots.png) part of the report, we observe that the Monte Carlo Tree Search agent beats the Monte Carlo Search agent when it goes first (MC manages a draw about a third of the time), and when MC goes first MCTS virtually always manages to get a draw.  
Both MCTS and MC beat the Random agent all of the time when they start. Random manages very few wins agains MC when it start, but none against MCTS.  

MCTS > MC > Random  
  
This is the logical outcome, as MCTS evaluates the possibilities of all possible moves -> Choose most strategic option -> Best outcome.  
MC lacks the tree based structure of MCTS: Relies on randomly simulating games -> Lack of planning compared to MCTS.  