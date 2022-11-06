# 🚀 Let us Exploit Reward Shifting in Value-Based Deep-RL!

### 🌐 [Project Page](https://sites.google.com/view/rewardshaping)

### Key Insight: A positive reward shifting leads to conservative exploitation, and a negative reward shifting leads to curiosity-driven exploration.


## 🏋️ Reproduction & Basic Usage: 

To reproduce our results, please follow instructions in each folder. 
Actually, the easiest way of reproduction is to play with reward shifting!

🧑🏻‍💻 In your tasks with value-based DRL, please just try to add a line right after the line of interaction with your environment, e.g., 

```next_s, r, done, info = env.step(a)```

```r = r + args.shifting_constant```

❕Don't forget to remove such a shift in evaluating your policy :) 

## 💡 Potential Ideas 


Here are several potential extensions of our work:
- Theoretically, the guidance of choosing shifting constant values.
- Methodologically, the choice of ensemble bias values
- Empirically, combining upper and lower bound (as non-linear combination) with Thompson Sampling for better exploration.
- Other linear reward shaping, e.g., with non-trivial scaling factor **k**.

## 📝 BibTex

```
@article{sun2022exploiting,
  title={Exploiting reward shifting in value-based deep rl},
  author={Sun, Hao and Han, Lei and Yang, Rui and Ma, Xiaoteng and Guo, Jian and Zhou, Bolei},
  journal={arXiv preprint arXiv:2209.07288},
  year={2022}}
