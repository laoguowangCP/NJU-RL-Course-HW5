# NJU Advanced-RL Course-HW5: Offline-RL
NJU Reinforcement Learning 2021 HW5 Archive

## What is it?
It's a continuous BCQ runner, using D4RL Hopper-v2 dataset, produce trained models.

## Install
Get D4RL Hopper-v2 dataset [here](https://github.com/rail-berkeley/d4rl), extract files in /dataset_mujoco directory.

I personally figured out how to make it works by using:
Ubuntu 18.04.2 LTS (Earlier versions may need further installation of OpenGL dependences)
Python3.6
Mujoco200_Linux (Refer to the installation instructions [here](https://github.com/openai/mujoco-py))
Mujoco-py\==2.0.2.5
numpy\==1.19.5 (Later versions may cause mismatch of size of numpy.ndarray)

## Run
```
python3 test_data.py
```

## Other tips may help
cannot find -lGL: [issue](https://github.com/openai/mujoco-py/issues/618)

No such file or directory 'patchelf' on mujoco-py installation: ```sudo apt-get install patchelf``` according to this [issue](https://github.com/openai/mujoco-py/issues/652)

GL/osmesa.h: No such file or directory: ```sudo apt install libosmesa6-dev libgl1-mesa-glx libglfw3``` according to this [issue](https://github.com/ethz-asl/reinmav-gym/issues/35), also see the [Ubuntu installtion troubleshooting](https://github.com/openai/mujoco-py#troubleshooting)

Missing path to your environment variable LD_LIBRARY_PATH: you can simply use sudo referring to this [issue](https://github.com/openai/mujoco-py/issues/619). If you're using conda, you need to clarify environment variable manually in shell, or configure it in Run/Debug configuration in PyCharm.

## Thanks
[sfujim](https://github.com/sfujim/BCQ)'s code for Batch-Constrained deep Q-Learning (BCQ)，and issues in [mujoco-py](https://github.com/openai/mujoco-py) .

## Reference
[1] Fujimoto S, Meger D, Precup D. Off-policy deep reinforcement learning without exploration[C]//International Conference on Machine Learning. PMLR, 2019: 2052-2062.
