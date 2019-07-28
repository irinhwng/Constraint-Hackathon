Slides: https://docs.google.com/presentation/d/1SpD1ySA8_fbrtzKZG4D1j4vtduBDNeT0NLZdanIxVek/edit#slide=id.g5d3e00cfa0_0_37

# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png)  Data Science Venn Diagram

The goal is to create the best performing model on a hold-out sample of data. The task is to predict if a person's income is in excess of $50,000 given certain profile information, and more specifically to generate predicted probabilities of income being **above** $50,000 for each row in the test set. This will simply be a csv with a single column of the probability  **_with 'wage' as a header_**.


This will be a constrained optimization. To understand what that means, let's take a look at the Project Management Venn Diagram, below.

![](https://berkonomics.com/wp-content/uploads/2015/11/goodfastcheap1-1.png)

The idea is that for any project you can have any two of these. You can have good work done cheap, but it will take a long time. You can have good work done fast, but it won't be cheap. Or you can have work done fast and on the cheap, but it won't be good.

Today we will apply this concept to data science.

I am given a dataset and teams will be randomly assigned to one constraint. My constraint is features; **I must only select 20 best features for my model of choice.** The notebook `Workflow.ipynb` shows how my team and I modeled the best model based on selecting a maximum of 20 features using sklearn's SelectKBest. 

**Note:** We were given 6 hours to submit our predictions. After the 6 hour period, we were given 30 minutes to create presentation slides. 

---

### Features Constraint
- Your choice of algorithm
- **Limited to a maximum of 20 features**
- Your choice of samples

---
## Conclusion
- Due to the time constraint of the hackathon, we couldn't execute Random Forest, ADA Boost, and Gradient Boost. Thus, we decided to move forward with the logistic regression with a log loss score of .344. 
- By using sklearn SelectKBest, we were able to find the 20 most favorable features. 
