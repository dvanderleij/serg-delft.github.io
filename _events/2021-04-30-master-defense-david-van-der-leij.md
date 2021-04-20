---
layout: event
title: "Master Thesis Defense on using machine learning for predicting refactoring opportunities in industry code"
categories: [events, defenses]
start: "09:30"
end: "12:00"
speaker: David van der Leij
where: Online (Zoom)
---

**Abstract**

Refactoring is the process of improving the structure of code without changing its functionality.
The process is beneficial for software quality but challenges remain for identifying refactoring opportunities.
This work employs machine learning to predict the application of the refactoring type Extract Method in an industry setting with the use of code quality metrics.

We detect 919 examples in industry code of Extract Method and 986 examples
where Extract Method was not applied and compare this to open-source code.
We find that feature distributions between industry and open-source code differ, especially in class-level metrics.

We train models to predict Extract Method in industry code and find that Random Forests perform best.
We find that class-level metrics are most important for the performance of these models.
We then investigate whether models trained on an open-source set generalize to an industry setting.
We find that, although less performant than a custom fit model, a Logistic Regression type model performs admirably.
Afterward, we examine whether these models perform on unseen industry projects by validating on projects excluded from the training set.
We find that average performance is decent but lower than when using the whole industry dataset or an open-source dataset for training.

Lastly, we conduct a blind user study in which we ask experts to judge predictions made by our best model.
We find that experts generally agree with the model's predictions.
In the case that experts agree with the model's prediction to apply Extract Method, they do so because of high code complexity.
When they agree with the model's prediction not to refactor they most frequently give the reason that the respective methods are already sufficiently understandable.
