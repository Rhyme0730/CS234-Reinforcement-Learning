# Installation

* Download and uncompress this archive onto the machine you are planning to use for Assignment 2. Make sure your current working directory is the directory containing this README file.

* For this assignment, we will be using environments from PyBullet, a free and open-source physics engine. As with all the assignments, we recommend using a Python `venv` or a `conda` environment to prevent dependency issues. For this assignment, you will need to use Python 3.9.

    * Install the requirements for this assignments.

    ```bash
    pip3 install setuptools==65.5.0 "wheel<0.40.0"
    pip3 install -r requirements.txt
    ```

    * If any of the above steps fail and you are unsure of how to debug the issue, please make a post on EdStem and we will try to assist you.

* After completing the assignment, you may submit your solutions to Gradescope. You can generate your submissions using:

```bash
bash collect_submission.sh
```



# How to Run This Code

```shell
python main.py --env-name ENV --seed SEED --METHOD
```

ENV: cartpole/pendulum/cheetah

SEED: 1/2/3

METHOD: baseline/no-baseline/ppo

(note: no-baseline is REINFORCE)

e.g. For cartpole

```shell
python main.py --env-name cartpole --seed 1 --ppo
```



For problem (d) 's plot,

```shell
python plot.py --env-name ENV --seeds SEEDS
```

Running this scripts requires you have run all method for specified ENV and SEEDS

e.g.

![](code\results\results-cartpole.png)