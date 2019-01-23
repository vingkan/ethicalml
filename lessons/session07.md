# Session 07: Rights

- (15 mins) Programming Demo
- (60 mins) Case Study

## (15 mins) Programming Demo

[Slides](https://docs.google.com/presentation/d/18YLnUL4r4q-bp9l8a9VynJb7gf0wXnyN8wnhBLyjTsg/edit#slide=id.g4c29fe321c_0_20) introduce basic ideas of reinforcement learning. Main ideas:

- In reinforcement learning, an agent choose actions based on its representation of the world. Those actions are met with rewards, helping the agent update its representation and determine what action to take next.
- The multi-armed bandit approach illustrates the tradeoff between gathering more information about which action reaps the best rewards (explore) and acting on a current belief about the best action (exploit).
- Three simple variants of the multi-armed bandit make the explore/exploit tradeoff in slightly different wants: the epsilon-greedy algorithm, the epsilon-first algorithm, and the epsilon-decay algorithm.
- The explore/exploit tradeoff is a mathematical manifestation of our the human conflict between wanting to rigorously and thoroughly study a phenomenon and wanting to utilize existing knowledge about the phenomenon for positive impact.

Share [the Jupyter notebook illustrating three variants of the multi-armed bandit](https://www.kaggle.com/vingkan/multi-armed-bandit) applied to deciding which advertisement to serve to website visitors. Explain that in a real world application of multi-armed bandit, counterfactual data about which advertisement a visitor might have clicked would not be available. Demonstrate how the epsilon-greedy algorithm chooses the “true” optimal advertisement for this dataset but the other two variants do not. Change the parameters of the epsilon-first and epsilon-decay algorithms until they also choose the “true” optimal advertisement.

Give students time to experiment with different parameters and distributions, as explained in the notebook. Consider a pair programming exercise or homework assignment to explore further.

## (60 mins) Case Study

Ask students to choose a discussion leader whose responsibilities include:

- Encourage participation from all table members
- Ensure discussion questions are answered beyond the superficial

The responsibilities for other table members include:

- Take turns reading parts of the case study
- Asking clarifying questions about the scenario
- Compare the perspectives of different table members and different stakeholders

Share [the case study from the Princeton Dialogues on AI and Ethics: Automated Healthcare App](https://aiethics.princeton.edu/wp-content/uploads/sites/587/2018/10/Princeton-AI-Ethics-Case-Study-1.pdf). The case study tells the story of a hospital research team that builds an an app called Charlie to help type 2 diabetes patients get better treatments. The case study explores the themes of legitimacy, paternalism, transparency, censorship, and inequality.

The case study involves a debate over whether or not the multi-armed bandit approach is an acceptable way to test the effectiveness of various diabetes treatments. Ask students to use their new knowledge of multi-armed bandit algorithms to critique the scenario.

This case study is an important part of the course because it shows that technology companies are not the only organizations that can make ethically dubious choices. Ask students to reflect: What rights should participants in a medical study have? What rights should a user of an app have? Are these different? How so?
