# ITSM Incident Management ML

## ABC Tech

## Project Summary

### Requirement
ABC Tech, a leading organization in the IT-enabled business sector for over a decade, manages approximately 22-25k IT incidents monthly. These incidents are handled using ITIL best practices, including incident management, problem management, change management, and configuration management. However, recent customer surveys indicate dissatisfaction with the incident management process. To address this, ABC Tech aims to leverage machine learning to enhance ITSM processes through predictive analytics and automation.

### Key Objectives
The project identifies four critical areas where machine learning can significantly improve ITSM processes:

1. **Predicting High-Priority Tickets**:
   - Identify priority 1 & 2 tickets in advance to enable preventive actions and reduce potential disruptions.
2. **Incident Volume Forecasting**:
   - Predict quarterly and annual incident volumes across different domains to optimize resource allocation and technology planning.
3. **Automated Ticket Tagging**:
   - Auto-assign tickets to the appropriate priority levels and departments to minimize delays caused by reassignments.
4. **Predicting Request for Change (RFC)**:
   - Anticipate changes and potential misconfigurations in ITSM assets to enhance system reliability.

### Analysis
The dataset includes ordinal, nominal, and categorical variables. Advanced data preprocessing techniques, such as label encoding and standardization, were applied to prepare the data for machine learning. Various algorithms were used to train predictive models, including:

- Support Vector Machine (SVM)
- Decision Tree
- Random Forest
- K-Nearest Neighbor (KNN)
- XGBoost Classifier
- Artificial Neural Networks (ANN)

For incident volume forecasting, time series analysis was performed using Statsmodels and Matplotlib.

### Approach
The analysis was divided into three focused areas:

1. **Priority Prediction**:
   - Predictor variables: Category, CI Category, CI Subcategory, and WBS.
   - Goal: Accurately predict high-priority tickets to enable proactive measures.

2. **RFC Prediction**:
   - Predictor variables: Category, CI Subcategory, WBS, Priority, Number of Related Interactions, and Related Incidents.
   - Goal: Anticipate RFC occurrences and misconfigurations.

3. **Incident Volume Forecasting**:
   - Predictor variable: Ticket opening time.
   - Goal: Forecast incident trends to enhance planning and preparedness.

### Implementation Steps
1. Imported data, libraries, and performed exploratory data analysis to address missing values.
2. Selected relevant features, applied label encoding for ordinal columns, and split data into training and testing sets.
3. Trained models using the specified algorithms and evaluated their accuracy.
4. Exported the model with the highest accuracy for deployment.
5. Conducted time series analysis for incident volume forecasting using ticket opening time.

### Results
1. **High-Priority Ticket Prediction**:
   - Achieved 98.5% accuracy using the Random Forest algorithm.
2. **RFC Prediction**:
   - RFC prediction accuracy was limited due to dataset constraints.
3. **Incident Volume Forecasting**:
   - Successfully visualized incident trends throughout the year using Matplotlib, enabling strategic resource planning.

### Conclusion
This project showcases the potential of machine learning in revolutionizing ITSM processes at ABC Tech. By implementing predictive and automated solutions, the organization can:

- Enhance customer satisfaction through proactive incident management.
- Optimize resource allocation and improve operational efficiency.
- Minimize delays and system disruptions, paving the way for improved service delivery and technological advancement.

