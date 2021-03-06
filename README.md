## 2P Point Mass LQ Zero-Sum Game (2D)

- python:
    - source: `./submodules/ilqgames-py-cpp/python/timing_two_player_point_mass.py`
    - time: 20.80ms
- C++:
    - source: `./submodules/ilqgames-py-cpp/timing/time_2p_pointmass.cpp`
    - bin: `./submodules/ilqgames-py-cpp/bin/timing/time_2p_pointmass`
    - time: 0.3487ms
- Julia:
    - source: `./submodules/iLQGames.jl/timing/time_2p_pointmass.jl`
    - time: 0.00439ms

## 3P Unicycle General-Sum Game (12D)

- python: (not comparable because different implementation (no line search etc.))
    - source: `./submodules/ilqgames-py-cpp/python/time_3p_unicycle.py`
    - time: N/A
        - no convergence in reasonable time scale
        - single iterate takes approx 4.25 seconds

- C++:
    - source:
        - `./submodules/ilqgames-py-cpp/timing/time_3p_unicycle.cpp`
        - `./submodules/ilqgames-py-cpp/src/three_player_unicycle_example.cpp`
    - bin: `./submodules/ilqgames-py-cpp/bin/timing/time_3p_unicycle`
    - time: 16.27ms
- Julia:
    - source: `./submodules/iLQGames.jl/timing/time_3p_unicycle.jl`
    - time:
        - nonlinear manual: 7.194ms
        - nonlinear AD:    63.570ms

## 3P Feedback Linearized Unicycle

- C++:
    - source:
        - `./submodules/ilqgames-py-cpp/timing/time_3p_unicycle.cpp`
        - `./submodules/ilqgames-py-cpp/src/three_player_flat_unicycle_example.cpp`
    - bin: `./submodules/ilqgames-py-cpp/bin/timing/time_3p_flat_unicycle`
    - time: 13.254ms

- Julia:
    - source: `./submodules/iLQGames.jl/timing/time_3p_unicycle.jl`
    - time:
        - feedback-linearization manual: 3.980ms
        - feedback-linearization AD:    52.503ms
