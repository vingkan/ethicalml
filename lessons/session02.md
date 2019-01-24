# Session 02: Data Preparation

- (30 mins) Programming Demonstration
- (20 mins) Mini Lecture
- (25 mins) Programming Demonstration

## (30 mins) Programming Demonstration

Share [the Jupyter notebook about data exploration](https://www.kaggle.com/vingkan/data-exploration). The notebook provides examples to:

- Load a dataset with Pandas
- Query records in a Pandas DataFrame
- Create a scatter plot with Pandas and Seaborn
- Create a bar plot with Pandas and Seaborn
- Create a histogram with Pandas and Seaborn

Review the questions that students brainstormed in the previous session. Choose questions that could be answered by a query, a scatter plot, a bar plot, or a histogram. For a plot, ask students to sketch what they think the result will look like. Then, demonstrate the code needed to produce the plot Probe students by asking if the result answers their question.

If time remains, ask students to modify the code examples to answer some of their other questions. Visit tables to support students or offer support while debugging. For questions that require more involved code than these samples, consider a homework assignment or a pair programming exercise.

## (20 mins) Mini Lecture

[Slides](https://docs.google.com/presentation/d/18YLnUL4r4q-bp9l8a9VynJb7gf0wXnyN8wnhBLyjTsg/edit#slide=id.g4bbf2d35b7_1_68) introduce basic ideas related to data preparation. Main ideas:

- For school or personal projects, you can find interesting open datasets on [Kaggle](https://www.kaggle.com/datasets), [the UCI machine learning repository](https://archive.ics.uci.edu/ml/datasets.html), or [government data portals](https://data.cityofchicago.org/).
- Real-world data is unruly: missing values, unstructured text, digitization errors.
- “Big data” concerns not just volume, also velocity and variety.
- If you are working with especially clean and meaningful data, seek to understand and respect the work that went into preparing it. It is not uncommon for organizations to outsource data labeling to people who can perform it quickly and cheaply.
- Data preparation influences the effectiveness of machine learning solutions as much, if not more, than the prediction algorithms do.
- “Feature engineering” is when machine learning engineers experiment with different ways of combining input data to improve model performance.
- Choosing an appropriate data type for a feature determines how a machine learning model will interpret values for that feature.
- Don’t hoard data: if your organization is collecting data, consider whether or not you need that data and how it might be misused or misrepresented.

Ask students to write down what data type they would use to represent each feature in the California housing prices dataset. If there seem to be disagreements over data types, ask for volunteers to share the reasoning behind competing choices.

## (25 mins) Programming Demonstration

Motivate data preparation for machine learning:

- What might we do with records that have missing values? Just discard them?
- Certain models are sensitive to the scale of features. Features such as median income may be weighted higher than say, number of rooms, simply because of the difference in scale between the values of the features.
- If the input features are not related to the output, no model or algorithm can save us. What features might we engineer that are not already in our dataset?

Share [the Jupyter notebook about data preparation](https://www.kaggle.com/vingkan/data-preparation). The notebook provides examples to:

- Encode categorical variables as one-hot binary variables using Pandas
- Impute missing values with different strategies using Scikit Learn
- Engineer new features using Pandas and Numpy
- Scale numerical features using Scikit Learn

[Slides](https://docs.google.com/presentation/d/18YLnUL4r4q-bp9l8a9VynJb7gf0wXnyN8wnhBLyjTsg/edit#slide=id.g4c29fe321c_1_80) include code examples and include links to the documentation.

**Next:** [Model Evaluation](session03.md)
