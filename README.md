# Deep Reinforcement Learning for Fano Hypersurfaces
We design a deep reinforcement learning algorithm to explore a high-dimensional integer lattice with sparse rewards, training a feedforward neural network as a dynamic search heuristic to steer exploration toward reward dense regions. We apply this to the discovery of Fano 4-fold hypersurfaces with terminal singularities, objects of central importance in algebraic geometry. Fano varieties with terminal singularities are fundamental building blocks of algebraic varieties, and explicit examples serve as a vital testing ground for the development and generalisation of theory. Despite decades of effort, the combinatorial intractability of the underlying search space has left this classification severely incomplete. Our reinforcement learning approach yields thousands of previously unknown examples, hundreds of which we show are inaccessible to known search methods.

This is the repository for the source code and data associated to the paper: 

*Deep Reinforcement Learning for Fano Hypersurfaces*, [arXiv](https://arxiv.org/abs/2603.15437)

## Code

**Exhaustive Search** 
- `fano_exhaustive.py` search code
- `fano_exhaustive_analysis.ipynb` analysis code
  
**Fixed Heuristic Search**
- `fano_main.py` search and analysis code
  
**Dynamic Heuristic (Deep Reinforcement Learning) Search**
- `fano_main.py` search and analysis code

## Data

All data from the experiments is already in the repository in the `/data` folder, except for the two searched point dataset files due to their size. These are hosted on [GitHub Releases](https://github.com/marctruter/deep_fano_hypersurface/releases) and can be downloaded directly via:
- [fixed_searched_points.csv](https://github.com/marctruter/deep_fano_hypersurface/releases/download/v1.0/fixed_searched_points.csv)
- [dynamic_searched_points_episode_1.csv](https://github.com/marctruter/deep_fano_hypersurface/releases/download/v1.0/dynamic_searched_points_episode_1.csv)

Place both files in the `/data` folder.

**Exhaustive Search**
- `/data/exhaustive_terminal_points.csv` terminal points found by the search
  
**Fixed Heuristic Search**
- `/data/fixed_settings.json` constants used
- `/data/fixed_terminal_points.csv` terminal points found by the search
- `/data/fixed_searched_points.csv` searched points
- `/data/fixed_reward_vs_steps.csv` number of terminal points found against step count
  
**Dynamic Heuristic (Deep Reinforcement Learning) Search**
- `/data/dynamic_settings.json` constants and hyperparameters used
- `/data/dynamic_terminal_points_episode_1.csv` terminal points found by the search
- `/data/dynamic_terminal_points_total.csv` terminal points over all episodes
- `/data/dynamic_searched_points_episode_1.csv` searched points
- `/data/dynamic_reward_vs_steps_episode_1.csv` number of terminal points found against step count
- `/data/dynamic_model.pth` neural network model at the final step of the search

**Other**
- `/data/qs_terminal.csv` classification of quasismooth terminal Fano 4-fold hypersurfaces with Fano index 1
- `/data/differing_points_fixed.csv` terminal points found in the fixed but not dynamic search
- `/data/differing_points_dynamic.csv` terminal points found in the dynamic but not fixed search
- `/data/differing_distances_fixed.csv` closest distances of terminal points found in the fixed but not dynamic search to their neighbours
- `/data/differing_distances_dynamic.csv` closest distances of terminal points found in the dynamic but not fixed search to their neighbours
