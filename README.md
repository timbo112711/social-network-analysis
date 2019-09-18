# Link Prediction in Social Email Network
## Goal
The goal here was to provide a use case of grabbing structured data and performing analysis with that structured data. Mapping each user's social email network and also trying to predict the probability of a link between a set of users.

### Data
The data was gathered from the Microsoft Graph API. Using this API we were able to gather all users, their inbox and sent email folders, and who they received and sent emails to.

    Steps:
    1. Grab all user's email (userPrincipalName)
    2. For each email grab their mailFolders
        a. Parse out the inbox ID and sent ID
    3. Create a df that holds each users email and their inbox ID
    4. 

### Workflow
1. Bring in raw data from MS Graph API
2. Clean up (formating, NA's, etc.)
3. EDA
4. Feature Engineering
5. Model
    - Split data into training and test sets
    - Use SVM or Logistic Regression 
        - These algo's are good for binary classification
        - Use metric report to a assess model performance (precision, recall, f1-score), confusion matrix, and ROC Curve. All of which will be explained in this section.
6. Results
7. Recommendation
