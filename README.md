# Steam Duck - PAWO (Personal Autonomous Walking Optimizer)

![PAWO Image](assets/images/robot.png)

I started the project at the end of November 2023 as my own version of the BDX Droid from Disney Imagineering. The original code name was **Steam Duck**, but for stylistic reasons I later renamed it after the mythical peacock (the star constellation *Pavo*). After that, I came up with an acronym, so the name became **P.A.W.O. (Personal Autonomous Walking Optimizer)**.

Finally, during an exhibition in Brno in October 2025, some students jokingly called the robot a **“futuristic chicken.”**

So yes — this project has had many names and versions. But no matter what the name is, it remains a very cool experiment in figuring out how to build a beautiful machine like the BDX Droid using only off-the-shelf components. The idea is to make it possible for anyone to build it with just 3D-printed parts, a screwdriver, and standard hobby-shop materials.


📺 [YouTube Channel](https://youtube.com/playlist?list=PLCrnO1B0KE3rKf2_9nu4y9VyF9zSY7Yt8&si=5LN6mWCUGIe7l07J) – See our robots in action!

☕ [Buy me a Coffee](https://www.vut.cz/en/people/stanislav-vechet-18462) at Laboratory of bio-inspired robotics, Institute of Autonomous Systems

# Steam Duck v1

First version of the droid with simple linkages, simple joints with hope everything will magicaly work...which wasn't.

![PAWO Image](assets/images/steamduckv1.png)

The main idea was to control the robot using PPO (Proximal Policy Optimization) which was also very naive to work in first place, even it does something.

# Steam Duck v2 - PAWO

The hardware for version 2 was completely redesigned, and we were able to create a simulation model in PyBullet that was accurate enough to experiment with several cyclic gait algorithms. This model is based on the version-1 geometry, but uses the updated dynamic parameters from version 2. The model still has 3 DOF per leg.
At this stage, we combined classic control algorithms—specifically a custom Raibert-style controller based on classical dynamics calculations—with reinforcement learning. The RL component used PPO from Stable Baselines3 along with a custom MPC module. Even though I wasn’t completely satisfied with the results, it somehow works. :)

[![Pawo Walking Twins](assets/images/PawoWalkingTwins.png)](https://raw.githubusercontent.com/St4nin/steam-duck-pawo/main/assets/videos/PawoWalkingTwins.mp4)


# Support

We appreciate if you cite one of this sources as support of our work. Thanks a lot.

## Citations

### Plain text

S. Vechet, J. Krejsa and K. -S. Chen, "Vertical Stabilization of Bipedal Walking Drone PAVO with Proximal Policy Optimization," 2024 21st International Conference on Mechatronics - Mechatronika (ME), Brno, Czech Republic, 2024, pp. 1-6, doi: 10.1109/ME61309.2024.10789752.

### BibTex

~~~
@INPROCEEDINGS{10789752,
  author={Vechet, Stanislav and Krejsa, Jiri and Chen, Kuo-Shen},
  booktitle={2024 21st International Conference on Mechatronics - Mechatronika (ME)}, 
  title={Vertical Stabilization of Bipedal Walking Drone PAVO with Proximal Policy Optimization}, 
  year={2024},
  volume={},
  number={},
  pages={1-6},
  keywords={Legged locomotion;Training;Mechatronics;Machine learning algorithms;Navigation;Reinforcement learning;Robots;Optimization;Faces;Drones;Machine Learning;Proximal Policy Optimization;Walking Robot;Biped Robot},
  doi={10.1109/ME61309.2024.10789752}}
~~~
