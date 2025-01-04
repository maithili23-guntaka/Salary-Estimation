# Salary-Estimation
Salary Estimation | K-nearest neighbour model
# Salary_Estimation-using-K-Nearest-Neighbour
1. Finding the Problem Application:
 * The goal is to predict whether a job applicant's previous salary was above or below $50k. This information can be useful for HR in various ways, such as salary negotiations and compensation planning.
2. Collecting Dataset:
 * The dataset will likely include features like:
   * Age
   * Education Level (represented as a numerical value)
   * Capital Gain
   * Hours Worked per Week
 * These features will be used to estimate the salary.
3. Load and Summarize Dataset:
 * The note mentions using the Pandas library to load the dataset from a CSV file.
 * Basic summary statistics, such as the number of rows and columns, will be calculated.
 * The first few rows of the dataset will be displayed for a quick overview.
4. Mapping Data from Text to Binary Number:
 * The target variable (salary above or below $50k) is likely stored as text in the dataset.
 * This step involves converting the text labels to binary values (e.g., 0 for <= $50k and 1 for > $50k). This is necessary for most machine learning algorithms.
5. Segregation Dataset to Train & Test
   iloc - It help us select Avalue that Belongs to Particular rows and columns
6. Splitting Data into Training and Testing Sets:
 * The dataset will be divided into two parts:
   * Training set: Used to train the K-Nearest Neighbors model.
   * Testing set: Used to evaluate the model's performance on unseen data.
7. Feature Scaling:
 * If the features have different scales (e.g., age vs. capital gain), scaling is often necessary to prevent features with larger values from dominating the distance calculations in K-Nearest Neighbors.
8. K-Nearest Neighbors Model:
 * The K-Nearest Neighbors algorithm will be used to build the predictive model.
 * The optimal value for the hyperparameter k (number of neighbors) will be determined using techniques like cross-validation.
9. Finding the Best K-value number of neighbors
 * choose the k value where we are getting least mean error
10. Traing
 * Training our model for prer-processed dataset model.fit(X_train,Y_test)
11. Validation
 * Obtaining the accurancy of the model
12. predicition
 *  Observing How our model is Classifying our new data
