# Session 05: Fairness I

- (15 mins) Mini Lecture
- (15 mins) Activity
- (45 mins) Programming Demo

## (15 mins) Mini Lecture

[Slides](https://docs.google.com/presentation/d/18YLnUL4r4q-bp9l8a9VynJb7gf0wXnyN8wnhBLyjTsg/edit#slide=id.g4c29fe321c_0_10) introduce three measures of fairness. Main ideas:

- There are hundreds, if not thousands, of measures of how fair a model is. As a machine learning practitioner, you must work with your team of stakeholders, users, and subject matter experts to determine which metrics are appropriate for your work.
- Many fairness metrics are based on the three in these slides: unawareness, demographic parity, and equality of opportunity.
- For a summary of these three metrics and others, see [Ziyuan Zhong’s article in Towards Data Science](https://towardsdatascience.com/a-tutorial-on-fairness-in-machine-learning-3ff8ba1040cb).
- Different fairness metrics compete with or contradict each other. It is mathematically impossible to satisfy all three of these fairness metrics at once, besides extreme cases.
- As a machine learning practitioner, you must be familiar with the laws, regulations, and protocols related to the project you are working on. Ethics of fairness go beyond just what laws require, extending into what fairness ought to mean for your stakeholders.

## (15 mins) Activity

Share the [interactive Google research demonstration: "Attacking discrimination with smarter machine learning"](http://research.google.com/bigpicture/attacking-discrimination-in-ml/) by Martin Wattenberg, Fernanda Viégas, and Moritz Hardt, based on the research of Moritz Hardt, Eric Price, and Nathan Srebro.

Visit student tables while they play with the activity. Possible questions for students:

- In this example, which group appears to be worse-off: orange or blue?
- Which metric of fairness do you think is best suited to to credit loans?

## (45 mins) Programming Demo

Introduce the next programming challenge, students will implement a machine learning system that decides which job applicants should advance to the interview stage based on the skills listed in their resume. Ask students to propose definitions of fairness suitable for this task.

Show students [the video explaining John Rawls’ thought experiment: the veil of ignorance](https://www.youtube.com/watch?v=A8GDEaJtbq4).

Explain that this activity will include a veil of ignorance: each student has been secretly assigned to one of the applicants in the test (hold-out) dataset. Students will not know who they are until after they have chosen their machine learning model. Then, the class will see how each team’s model rated their persona in this hypothetical world.

Share [the dataset on Kaggle](https://www.kaggle.com/vingkan/strategeion-resume-skills/home). Ask students if this data is suitable for machine learning.

Share [the Jupyter notebook called Strategeion Resumes Starter](https://www.kaggle.com/vingkan/strategeion-resumes-starter) that loads the dataset. Remind students how to train and evaluate models with Scikit Learn. Demonstrate a simple classifier and how to calculate each of the three fairness metrics covered in the session.

Consider having a pair programming activity or homework assignment where students try to build and the select the best hiring model they can. Remind the class that they will find out which applicant in the test (hold out) data represents them, after the veil of ignorance is lifted at the start of the next session.

**Next:** [Fairness II](session06.md)
