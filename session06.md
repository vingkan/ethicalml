# Session 06: Fairness II

- (15 mins) Review
- (60 mins) Case Study

## (15 mins) Review

Before the session, send each student their unique code that corresponds to one of the applicants in the test (hold out) set of resumes. Choose a few of the students’ classifiers and show the class how each classifier ranks their veil of ignorance personas. Ask for students reactions: Did any of the issues you sought to prevent come to pass?

To prepare for the case study, review the logistic regression model. [Slides](https://docs.google.com/presentation/d/18YLnUL4r4q-bp9l8a9VynJb7gf0wXnyN8wnhBLyjTsg/edit#slide=id.g4c29fe321c_0_15) include main ideas:

- Logistic regression outputs a probability based on the weighted sum of predictors.
- Students can see how changing the weights of a logistic regression changes the curve in [the Desmos plot](https://www.desmos.com/calculator/bpmf2dzwbc).

## (60 mins) Case Study

Ask students to choose a discussion leader whose responsibilities include:

- Encourage participation from all table members
- Ensure discussion questions are answered beyond the superficial

The responsibilities for other table members include:

- Take turns reading parts of the case study
- Asking clarifying questions about the scenario
- Compare the perspectives of different table members and different stakeholders

Share [the case study from the Princeton Dialogues on AI and Ethics: Hiring By Machine](https://aiethics.princeton.edu/wp-content/uploads/sites/587/2018/12/Princeton-AI-Ethics-Case-Study-5.pdf). The case study tells the story of a company called Strategeion that, overwhelmed by a glut of resumes, decides to build a machine learning system called PARiS to identify which job applicants should advance to an interview. The case study explores the themes of fairness, irreconcilability, diversity, capabilities, and contextual integrity.

Prior to discussion question three in the case study, students learn of a complaint from an applicant who was automatically rejected, but otherwise qualified for an interview. The algorithm’s developers offer an explanation for the rejection. Ask students to reflect: Do you find the developers’ explanation of the rejection compelling?

Share [the Jupyter notebook called PARiS Classifier](https://www.kaggle.com/vingkan/paris-classifier). This notebook includes a working version of the resume classifier with the training and pilot data loaded. Ask students to explore the classifier and determine whether or not the developers came to the right conclusion. Inform students that the PARiS classifier is a logistic regression model and ask them to use what they learned about logistic regression to investigate the developer’s conclusion.
