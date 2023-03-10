# Mushroom Classification: Safe to eat or deadly poison?


**Context**

Although this dataset was originally contributed to the UCI Machine Learning repository nearly 30 years ago, mushroom hunting (otherwise known as "shrooming") is enjoying new peaks in popularity. Learn which features spell certain death and which are most palatable in this dataset of mushroom characteristics. And how certain can your model be?

**Content**

This dataset includes descriptions of hypothetical samples corresponding to 23 species of gilled mushrooms in the Agaricus and Lepiota Family Mushroom drawn from The Audubon Society Field Guide to North American Mushrooms (1981). Each species is identified as definitely edible, definitely poisonous, or of unknown edibility and not recommended. This latter class was combined with the poisonous one. The Guide clearly states that there is no simple rule for determining the edibility of a mushroom; no rule like "leaflets three, let it be'' for Poisonous Oak and Ivy.

**Solution and results**

In this binary classification problem since the poisonus class is the positive class we aim to maximize recall in order to avoid false negatives, i.e. people getting poisoned by eating misclassiefied mushrooms. Due to the high number of nominal variables we solve the problem through random forests achieving a perfect classification on the test set with grid search cross validation.
