# NJU-RL-Course-HW5-Offline-RL
NJU Reinforcement Learning 2021 HW5 Archive

## What is it?
It's a BCQ runner, using D4RL Hopper-v2 dataset, produce trained models.

## Install
Get D4RL Hopper-v2 dataset [here](https://github.com/rail-berkeley/d4rl)

I personally figured out how to make Mujoco works by using:
Ubuntu 18.04.2 LTS (Earlier versions may need further installation of OpenGL dependences)
Python3.6
Mujoco200_Linux (Refer to the installation instructions [here](https://github.com/openai/mujoco-py))
Mujoco-py\==2.0.2.5
numpy\==1.19.5

## Run
```
python3 test_data.py
```

## Thanks
To [sfujim](https://github.com/sfujim/BCQ)'s code for Batch-Constrained deep Q-Learning (BCQ)，and issues in [mujoco-py](https://github.com/openai/mujoco-py) .

## Reference
[1] Fujimoto S, Meger D, Precup D. Off-policy deep reinforcement learning without exploration[C]//International Conference on Machine Learning. PMLR, 2019: 2052-2062.
