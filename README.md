# Deep Reinforcement Learning for Fano Hypersurfaces
We design a deep reinforcement learning algorithm to explore a high-dimensional integer lattice with sparse rewards, training a feedforward neural network as a dynamic search heuristic to steer exploration toward reward dense regions. We apply this to the discovery of Fano $4$-fold hypersurfaces with terminal singularities, objects of central importance in algebraic geometry. Fano varieties with terminal singularities are fundamental building blocks of algebraic varieties, and explicit examples serve as a vital testing ground for the development and generalisation of theory. Despite decades of effort, the combinatorial intractability of the underlying search space has left this classification severely incomplete. Our reinforcement learning approach yields thousands of previously unknown examples, hundreds of which we show are inaccessible to known search methods.

## Data
All data from the experiments is already in the repository, except for the two searched point dataset files due to their size. These are hosted on [GitHub Releases](https://github.com/marctruter/deep_fano_hypersurface/releases) and can be downloaded directly via:
- [fixed_searched_points.csv](https://github.com/marctruter/deep_fano_hypersurface/releases/download/v1.0/fixed_searched_points.csv)
- [dynamic_searched_points_episode_1.csv](https://github.com/marctruter/deep_fano_hypersurface/releases/download/v1.0/dynamic_searched_points_episode_1.csv)

Place both files in the `/data` folder.

