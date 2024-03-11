# Flood-Prediction-

We are going to predict flood occurance based on rainfall.
Predicting floods using historical rainfall data is essential for providing early warnings to communities, allowing them to evacuate and take necessary precautions ahead of time. This predictive capability enables efficient allocation of resources, facilitates community preparedness efforts, and supports the development of resilient infrastructure to mitigate the socioeconomic impacts of flooding and enhance disaster management and mitigation strategies. By leveraging advanced forecasting techniques and data-driven approaches, authorities can minimize loss of life, property damage, and economic disruption associated with flood events, ultimately contributing to safer and more resilient communities.
I have completed a project for the analysis of flood data and flood occurrence prediction. I began by importing relevant libraries, then proceeded to read the data. I checked whether it was clean or not, and fortunately, it was clean without any null or inappropriate values. Upon checking the difference between the mean and 50th percentile in the describe function output, I noticed many outliers. However, I decided not to treat them as they are relevant in this case.
Features: Monthly rainfall on all the 12 months,Year, annual rainfall, flood occurrence (binary: 1 for flood, 0 for no flood).

I found the values of each feature for the minimum and maximum amount of rainfall. Then, I applied conditional probabilities for flood occurrence when rainfall density was more than 500 during the months of June, July, and August, as values above 500 were only found when rainfall density was less than 500 for all other months.

Next, I took the correlation matrix and found that there is a positive correlation between annual rainfall and floods. I then plotted a bar plot for average annual rainfall for floods and histograms for all features. Additionally, I created a bar plot of flood occurrence over the years and a pie chart on the count of floods from 1901 to 2018.

Moving on to model building, I defined features and target values, and converted categorical values to numerical using label encoder. I performed feature scaling using standard scalar and split the data into training and test sets. I imported models including logistic regression, SVC, KNeighborsClassifier, Random Forest Classifier, and Decision Tree.

I compared the models with cross-validation and found that the Random Forest Classifier performed the best in terms of accuracy, precision, F1 score, and recall. Consequently, I chose it and trained it with the training data to make predictions.

I also created a Power BI report for flood analysis.

Key conclusions: Flood occurrence is mainly dependent on annual rainfall, with a positive correlation between the two. The Random Forest Classifier proved to be the best model for prediction.
