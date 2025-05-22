# Berkeley-AI-ML-Capstone-Assignment-20.1
Initial Report and Exploratory Data Analysis (EDA)
### Project Title
Prediction for potential hotel booking cancellation prior to check-in
**Author**
Yu-Shen (Ethan) Tsao
#### Objective
The goal of this analysis to perform analysis on hotel booking transaction and make prediction on whether a booking will be likely to be canceled prior to check in


#### Rationale
Predicting hotel booking cancellations is crucial for optimizing revenue management and operational efficiency. Cancellations disrupt planning, leading to lost revenue and resource misallocation. By identifying likely cancellations in advance, hotels can implement proactive strategies such as overbooking, targeted promotions, or deposit requirements to mitigate risk. This enables better forecasting, improves room utilization, and enhances overall guest satisfaction through more reliable service planning.

#### Research Question
What are you trying to answer?
The primary research question of this study is: Can we accurately predict whether a hotel booking will be canceled based on customer, booking, and stay-related features? Using the Hotel Booking Demand dataset, this research aims to uncover key patterns and variables that influence booking cancellations. By developing a predictive model, we seek to help hotels identify high-risk reservations early, allowing them to take preventive actions to reduce last-minute cancellations and improve operational planning.

#### Data Sources
Hotel Booking Demand from Kaggle
https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand?resource=download&select=hotel_bookings.csv

#### Methodology
1. Clean the data starting from describing the data in phthon
2. Handeling missing values / drop useless columns that contains mostly NULL value
3. Create calcuations: to compute Total nights and Arrival Time
4. Use a Heatmap to identify which columns are strongly correlated to the cancallation field
5. Use Logistic Regression Model to make prediction on cancellation 

#### Results
About 80% of the time, the model correctly predicted whether a booking would be canceled or not.

Confusion Matrix: 
    True Positives (TP): Model correctly predicted cancellations (4761 times)
    False Negatives (FN): Model missed cancellations (4084 times)

Classification Report:
    Class 0 – Not Canceled:
        Precision (0.78): Of all bookings the model predicted as not canceled, 78% were actually not canceled.
        Recall (0.95): Of all bookings that were truly not canceled, 95% were correctly identified.
        F1-score (0.86): High score reflects strong model performance on this class.
     Class 1 – Canceled:
        Precision (0.86): When the model predicts a booking will cancel, it's correct 86% of the time.
        Recall (0.54): But it only catches 54% of actual cancellations — meaning it misses nearly half of them.
        F1-score (0.66): Moderate balance between precision and recall.


#### Next steps
Use additional classification algorithms such as KNeighborsClassifier, DecisionTreeClassifier or SVM  to determine and achieve higher accuracy scores




##### Contact and Further Information
