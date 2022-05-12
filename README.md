## AIM 5014 Reinforcement Learning - Spring 2022
## Aishwarya Singh

# Mini-Project: The LoCA Regret
## A Consistent Metric to Evaluate Model-Based Behavior in Reinforcement Learning

### Experiment

See Report. This code runs experiments for the tabular version of the LoCA test, based on a gridworld with edge rewards labeled T1 and T2. Task A and Task B have the same transition dynamics, but the reward function is locally different. A LoCA pretraining experiment consists of first training a method on Task A, followed by local training around T1 of Task B. After pretraining, the agent is trained and evaluated on the full environment of Task B. The additional training a method needs before it has fully adapted to Task B determines the size of the LoCA regret.

Control experiments without LoCA pretraining are simply trained and evaluated on Task B directly.
 
### Requirements:

This code is tested with Python 3.7. It utilizes packages found in a default Anaconda installation: numpy and matplotlib.

### Usage:

Use these commands to run the training or plot the results.
* Training: ```python main.py ```
* Visualize results : ```python visualize.py```

### Citation:

Code is adapted from work by Harm van Seijen et. al. at Microsoft, 2020.
```
@misc{seijen2020loca,
    title={The LoCA Regret: A Consistent Metric to Evaluate Model-Based Behavior in Reinforcement Learning},
    author={Harm van Seijen and Hadi Nekoei and Evan Racah and Sarath Chandar},
    year={2020},
    eprint={2007.03158},
    archivePrefix={arXiv},
    primaryClass={cs.LG}
}
```
<br/>

