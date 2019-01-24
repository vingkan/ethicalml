# Session 03: Model Evaluation

- (20 mins) Mini Lecture
- (40 mins) Programming Demo
- (15 mins) Competition

## (20 mins) Mini Lecture

[Slides](https://docs.google.com/presentation/d/18YLnUL4r4q-bp9l8a9VynJb7gf0wXnyN8wnhBLyjTsg/edit#slide=id.g4c29fe321c_0_0) introduce basic metrics for model evaluation. Main ideas:

- Split the dataset into training and test (hold-out) sets. Split the training set into training and validation sets. Training data is used to determine model weights. Validation data is used to evaluate and compare model performance. Test data helps check how well the model might generalize to future data.
- The confusion matrix compares a model’s predictions to the actual classes of the data.
- Classification accuracy is not a helpful metric when the class distribution is imbalanced.
- Instead, use recall and precision, which are summarised by the F1-score.

## (40 mins) Programming Demo

Share [the Jupyter notebook about model evaluation](https://www.kaggle.com/vingkan/model-evaluation). The notebook provides examples to:

- Split data into training and validation sets with Pandas and Scikit Learn
- Train and evaluate a k-nearest neighbors classifier with Scikit Learn
- Train and evaluate a decision tree classifier with Scikit Learn
- Train and evaluate a logistic regression classifier with Scikit Learn
- Submit predictions to a Kaggle competition

The slides summarize how each of these three classifiers train and predict. The slides also suggest some parameters to tweak for each classifier and include links to the documentation.

Ask students to try different models and parameters. Visit tables to support students or offer support while debugging. Probe students by asking them to compare two different models or two different versions of the same model.

## (15 mins) Competition

Remind students of the final deadline for submissions to the house prices prediction competition. If students are anxious about their programming skills, emphasize that programming is not the only important skill for machine learning: data preparation, feature engineering, and model selection will give their team an edge.

Consider asking students to write a short reflection. After completing the competition, do you feel that estimating home values is a suitable task for machine learning? Is the F1-score, on its own, a good metric for this competition?

**Next:** [Utility](session04.md)
