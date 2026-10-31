# Factor Detection Task of Cyberbullying Using the Deep Learning Model

Instead of only asking whether a comment is cyberbullying, this work detects the *factors* that make it up: intimidation, harassment, insult, sarcasm, arousal, and valence.

* Factor Detection Task of Cyberbullying Using the Deep Learning Model
* Yu-Hsuan Wu, Sheng-Wei Huang, **Wei-Yi Chung**, Chen-Chia Yu, Jheng-Long Wu
* 2022 IEEE International Conference on Big Data (Big Data) Workshop, pp. 4323–4329
* [Paper](https://doi.org/10.1109/BigData55660.2022.10020779) | [Slides](./BigD809.pdf) | Blog walkthrough: [Cyberbullying factors](https://h30306.github.io/blog/paper/2022-ieee-bigdata-cyberbullying-factor-detection/)

This repository holds the presentation slides only. The model code and the annotated corpus are not published.

## Summary

1. **Six factors** with annotation guidelines: intimidation, harassment, insult, sarcasm, arousal, and valence.
2. **Chinese corpus**: 5,926 PTT comments labeled by three annotators. The labels are highly imbalanced (48 intimidation vs. 3,641 sarcasm and 2,175 harassment).
3. **Models**: one BERT classifier per factor; `h_CLS` goes through `softmax(W·h_CLS + b)`, fine-tuned end to end with cross-entropy.
4. **Case studies**: the trained classifiers label large-scale PTT discussions about public figures to show how the mix of factors shifts over time.

## Citation

```bibtex
@inproceedings{wu2022factor,
  title     = {Factor Detection Task of Cyberbullying Using the Deep Learning Model},
  author    = {Wu, Yu-Hsuan and Huang, Sheng-Wei and Chung, Wei-Yi and Yu, Chen-Chia and Wu, Jheng-Long},
  booktitle = {2022 IEEE International Conference on Big Data (Big Data)},
  pages     = {4323--4329},
  year      = {2022},
  doi       = {10.1109/BigData55660.2022.10020779}
}
```
