# CIS 5450 Final Project: Flight Cancellations
## Part I: Introduction and Setup
* Introduce the problem: Explain why predicting flight cancellations is important and how it can benefit airlines and passengers.
* Data source: Briefly describe the dataset, its features, and where it was obtained.
* Libraries: Import necessary Python libraries.
## Part II: Preprocessing
* Handle missing data: Check for missing values and decide on an appropriate strategy (imputation or removal).
* Data types: Ensure that each feature has the correct data type.
* Convert categorical variables: If needed, convert categorical variables into a format suitable for machine learning models (e.g., one-hot encoding).
* Handle datetime variables: Extract relevant information from datetime variables.
## Part III: Exploratory Analysis
* Descriptive statistics: Provide summary statistics for key features.
* Visualizations: Create visualizations to explore the distribution of flight cancellations, relationships between variables, and any patterns.
## Part IV: Data Wrangling and Staging
* Remove irrelevant columns: Drop columns that are not useful for modeling.
* Split the data: Divide the dataset into training and testing sets.
## Part V: Modeling
* Choose classification models: Consider including models like Logistic Regression, Decision Trees, Random Forest, Support Vector Machines, and Gradient Boosting.
* Train and evaluate models: Implement and evaluate each model using appropriate metrics (accuracy, precision, recall, F1-score).
* Discuss results: Compare the performance of different models and discuss their strengths and weaknesses.
## Part VI: Feature Engineering
* Create new features: Explore possibilities for creating new features that might enhance model performance.
* Feature scaling: If applicable, scale numerical features to a standard range.
## Part VII: More Modeling
* Fine-tuning: Perform hyperparameter tuning on the best-performing models.
* Ensemble methods: Consider using ensemble methods like stacking or bagging to improve predictive performance.
## Part VIII: Conclusion
**In summary:**
1. We conducted an exploratory data analysis to understand the relationship between various flight data features and the likelihood of flight delays. To do this, we modified our original dataframe to include a new 'Delayed' variable, classifying flights as delayed or not. Our first approach was using a Naive Gaussian Bayes model, which yielded a 72% accuracy in delay classification.
1. Seeking improvement, we then experimented with a basic neural network (NN). This NN, initially simple with just a few layers, showed promise after a few epochs, reaching an accuracy of 81%. However, upon fine-tuning the model by adjusting the learning rate and adding more layers for complexity, the accuracy slightly decreased to 79%. Interestingly, this model demonstrated a better learning trajectory, starting from 68% accuracy, compared to the initial model's 79% in the first epoch.
1. We also tried Random Forest Classification on our updated dataframe, which included the 'Delayed' boolean variable. This model achieved a 68% accuracy on the training set. While not exceptionally high, this accuracy was a meaningful baseline, considering the complexities of predicting real-world outcomes like flight delays. We acknowledged the limitations of our approach and considered exploring Gradient Boosting or more advanced deep learning methods in future iterations to potentially enhance accuracy.

**In the future:**
1. We could have included more datasets which detailed other potential confounding factors, such as the weather conditions of the various airports so we could have further examined if there was a relation between the airport's weather conditions and whether the flight is canceled or delayed.
1. In addition, we can further explore the use of more complex neural networks as classification models. These more advanced models could potentially lead to higher accuracy results.

**Overall Experience + Team Reflection:**
1. This was a great experience to finally apply what we learned in this class without having an outline given to us for what to do. We were able to fully utilize our creativity and delve into a topic and examine relationships using what we learned in the class.
1. It was an interesting experience to see how different models can give us different accuracies in each scenario and how no singular model will always be the most accurate for each scenario.
1. It was difficult at times as getting accurate predictions in this case was often more difficult than in class where the models are hand picked for us to get a certain conclusion. This shows how it is much more difficult and different in real life when we are looking for a conclusion and do not have one guaranteed.
