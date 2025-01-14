# CloudGroup-12

## Table of Contents
1. [Project Scope](#project-scope)
   - [Specific Problem](#specific-problem)
   - [Domain](#domain)
2. [Literature Review](#literature-review)
3. [Data Source(s)](#data-sources)
4. [Domain-specific Challenges](#domain-specific-challenges)
5. [KPI’s](#kpis)
6. [Deliverable -2](#deliverable---2)
   - [Data Understanding](#data-understanding)
   - [AWS Pipeline / Solution Chart](#aws-pipeline-solution-chart)
   - [Aws Glue Pipeline](#aws-glue-pipeline)
   - [AWS Athena](#aws-athena)
   - [AWS Quicksight](#aws-quicksight)
   - [AWS S3](#aws-s3)
7. [Deliverable 3](#deliverable---3)
   - [Data Sources](#data-sources)
   - [Data Preprocessing](#data-preprocessing)
   - [Model Training and development](#model-development-and-traning)
   - [Evaluation and Validation](#evaluation-and-validation)
   - [Screenshots](#screenshots)

## Project Scope

### Specific Problem
The project aims to predict and understand factors influencing passenger satisfaction, aligning with educational goals related to machine learning and data analytics with practical applications in customer service and business strategy.

### Domain
- **Industry:** Airline industry
- **Stakeholders:** Passengers, airline companies, regulatory bodies, and service providers within airports.

## Literature Review
Conduct a literature review of research papers, case studies, articles, and books related to the chosen domain. The purpose is to stay informed about the latest advancements and best practices in the field. Sources should be current and at least 5 sources should be documented and summarized.

## Data Source(s)
The potential data sources include:
1. [Airline Passenger Satisfaction | Kaggle](https://www.kaggle.com/datasets/teejmahal20/airline-passenger-satisfaction)
This dataset on Kaggle contains customer satisfaction scores from airline passengers.
2. [Airlines - The American Customer Satisfaction Index](https://theacsi.org/industries/travel/airlines/)
The American Customer Satisfaction Index: The American Customer Satisfaction Index provides a definitive measure of passenger satisfaction with cause-and-effect analysis. It includes data from 9 major airlines, plus an aggregate of smaller carriers. The 2023 results are based on data collected from April 2022 to March 2023.
3. [Maven Churn Challenge | Maven Analytics](https://mavenanalytics.io/blog/maven-airlines-challenge)
This dataset includes airline satisfaction scores for 129,880 passengers. Each record represents one passenger and contains details about passenger demographics, flight distance and delays, travel class and purpose, and ratings for factors like cleanliness, comfort, and service, as well as overall satisfaction with the airline.

## Domain-specific Challenges
- Data Integration: Integrating data from different sources like customer feedback surveys, social media sentiment analysis, operational flight data, and third-party service ratings can be challenging due to the heterogeneity of data. Each source may have its own format, structure, and quality, requiring significant preprocessing and cleaning efforts.

- Privacy Concerns: Collecting and analyzing data related to airline passenger satisfaction may involve handling sensitive personal information. Ensuring the privacy and anonymity of individuals while maintaining the utility of the data can be a significant challenge.

- Real-Time Analysis: The need for real-time analysis can pose a challenge, especially when dealing with large volumes of data or when the data is streaming in nature, such as social media sentiment analysis.

- Data Quality: The quality of data collected from sources like social media or customer feedback surveys can vary greatly. Issues such as bias in responses, missing data, or inaccurate data can impact the reliability of the analysis.


## KPI’s
Key Performance Indicators (KPIs) in this context would encompass the utilization of data attributes, the extent of data preprocessing, and the diversity of the dataset. It's crucial to have a wide-ranging dataset for robust analysis. Another significant KPI involves experimenting with various machine learning algorithms to identify the one that delivers the best performance. The optimal model would be the one that most accurately predicts or classifies according to the problem at hand. These KPIs collectively contribute to the successful analysis of airline passenger satisfaction.

## Deliverable - 2

The dataset is centered on airline passenger satisfaction, encompassing a range of attributes such as gender, age, customer type, travel class, and flight distance. It differentiates types of travel into personal and business categories. The dataset offers detailed ratings for various services, including inflight wifi, seat comfort, food and drink, and cleanliness. Additionally, it provides ratings for specific services like inflight entertainment, on-board service, leg room service, baggage handling, check-in service, and inflight service, presenting a comprehensive view of the passenger's travel experience.

Flight delays are recorded in terms of departure and arrival delay minutes, shedding light on their impact on passenger satisfaction. The overall satisfaction level of passengers is categorized as either 'satisfied' or 'neutral or dissatisfied'. This data is crucial for airlines to analyze and predict factors influencing passenger satisfaction, making it an essential tool for market research, customer experience management, and service quality improvement in the aviation industry. The dataset's comprehensive nature makes it invaluable for understanding passenger preferences and improving airline services.

### Data Understanding
We employed AWS Glue for schema discovery and data type definition, ensuring our dataset's structure was accurately recognized and categorized. Then we used Glue crawler for refining the dataset schema, allowing for precise categorization and organization of data fields. For in-depth querying and extracting insights, AWS Athena was used. This enabled us to perform comprehensive data analysis efficiently, allowing for complex queries and data aggregations.This approach not only streamlined our data analysis process but also enhanced the accuracy and relevance of the insights gained, proving crucial for informed decision-making and strategic planning Additionally, we utilized AWS QuickSight for data visualization. QuickSight's powerful visualization tools provided an intuitive interface for exploring and presenting the data, making it easier to identify patterns, trends, and correlations. This visual approach to data analysis enhanced our ability to gain insights, allowing us to make more informed decisions and develop effective strategies based on the dataset.

### AWS PIPELINE / SOLUTION CHART

<img width="807" alt="AWS Pipeline : Solution Chart" src="https://github.com/Datta9/CloudGroup-12/assets/115682022/430c6193-b812-44e7-bc3c-4dd09a884f4f">


### AWS GLUE PIPELINE
![Glue pipline](https://github.com/Datta9/CloudGroup-12/assets/116744004/89c16af9-f4ba-4944-8202-fc9fbc26b445)

### AWS ATHENA
![Query1](https://github.com/Datta9/CloudGroup-12/assets/116744004/b6ca58ce-5cdb-4587-91a0-c58ba4f3e7b1)
![Query2](https://github.com/Datta9/CloudGroup-12/assets/116744004/bca5ff38-45b6-4fb7-ab48-9d854e708820)
![Query3](https://github.com/Datta9/CloudGroup-12/assets/116744004/d356b7c6-1309-4f2b-aaca-01946e0db61d)
![Query4](https://github.com/Datta9/CloudGroup-12/assets/116744004/40c46523-1e7f-410d-9d42-dac68898634a)
![Query5](https://github.com/Datta9/CloudGroup-12/assets/116744004/3c318720-0012-45aa-bab5-075c0e339d7c)

### AWS QUICKSIGHT
![Visualization](https://github.com/Datta9/CloudGroup-12/assets/116744004/fe47f0f7-b3b3-418a-b658-7593043d29ce)
![Visualization 2](https://github.com/Datta9/CloudGroup-12/assets/116744004/b992a738-122d-4eed-82c4-dfa055edcea5)

### AWS S3
![S3](https://github.com/Datta9/CloudGroup-12/assets/116744004/a015c84a-5105-4621-a736-482875862306)

## DELIVERABLE - 3
The following machine learning frameworks and libraries are utilized in this project:

- AWS SageMaker: Used for managing the machine learning lifecycle, storing datasets, and potential hyperparameter tuning.
- TensorFlow: Employed for model development and training.
- scikit-learn: Utilized for data preprocessing, standardization, and evaluation metrics.
- XGBoost: Implemented for training a gradient boosting model.
- Random Forest (scikit-learn): Used for training an ensemble learning model.

### Data Sources
- Training Data: s3://airlinesatisfaction/data/train.csv
- Test Data: s3://airlinesatisfaction/data/test.

The dataset used for this project is stored in Amazon S3, a scalable object storage service provided by AWS. The training data is located at s3://airlinesatisfaction/data/train.csv, and the test data is located at s3://airlinesatisfaction/data/test.csv. Leveraging S3 allows for efficient data storage, retrieval, and management, providing a scalable and secure solution for handling large datasets.

### Data Preprocessing
Data preprocessing is a crucial step in preparing the dataset for model training. In this project, the following steps are performed:

- Handling Missing Values: Any missing values in the dataset are addressed, ensuring that the data used for training and testing is complete.

- Dropping Unnecessary Columns: Columns such as "Unnamed: 0" and "id" are dropped as they do not contribute to the predictive modeling.

- Encoding Categorical Variables: Dummy variables are created for categorical features like "Type of Travel" and "Class." This process involves converting categorical variables into numerical representations to facilitate model training.

- Gender and Customer Type Encoding: Specific categorical features like "Gender" and "Customer Type" are encoded to numerical values, providing a standardized format for the machine learning models.

### Model Development and Traning
Two machine learning models, XGBoost and Random Forest, are explored for this project:

- XGBoost: A powerful and scalable gradient boosting algorithm, XGBoost is employed for its efficiency in handling large datasets and its ability to capture complex relationships within the data.

- Random Forest (scikit-learn): Random Forest, an ensemble learning method, is used for training a model that combines multiple decision trees. This approach helps to enhance predictive performance and reduce overfitting.

The dataset is split into training and test sets to enable the models to learn from one subset and validate their performance on another.

### Evaluation and Validation
Model performance is assessed using various metrics:

- Accuracy Score: This metric provides an overall measure of how correct the model's predictions are. It is calculated as the ratio of correctly predicted instances to the total instances.

- Confusion Matrix: The confusion matrix provides a detailed breakdown of the model's performance, showing the number of true positives, true negatives, false positives, and false negatives. This matrix is particularly useful for understanding the model's ability to correctly classify instances.

Visualizations, including count plots, histograms, and heatmaps, are employed to gain additional insights into the data distribution and the models' predictions. These visualizations help in understanding potential patterns, trends, and areas where the models may excel or struggle.

### Screenshots
![Sagemaker-Train Data](https://github.com/Datta9/CloudGroup-12/blob/main/Screenshots/sagemaker%20l1.png?raw=true)

![Sagemaker-Airline Satifaction Plot](https://github.com/Datta9/CloudGroup-12/blob/main/Screenshots/sagemaker%20l2.png?raw=true)

![Sagemaker-Histogram:Age](https://github.com/Datta9/CloudGroup-12/blob/main/Screenshots/sagemaker%20l3.png?raw=true)

![Sagemaker-Inflight WIFI service](https://github.com/Datta9/CloudGroup-12/blob/main/Screenshots/sagemaker%20l4.png?raw=true)

![Sagemaker-Confusion Matrix](https://github.com/Datta9/CloudGroup-12/blob/main/Screenshots/sagemaker%20l5.png?raw=true)
![Sagemaker-Evaluation Metric1](https://github.com/Datta9/CloudGroup-12/blob/main/Screenshots/eval_metric.png?raw=true)
![Sagemaker-Evaluation Metric2](https://github.com/Datta9/CloudGroup-12/blob/main/Screenshots/eval_metrc2.png?raw=true)
![Sagemaker-ROC Curve](https://github.com/Datta9/CloudGroup-12/blob/main/Screenshots/roc_curve.png?raw=true)
###Deployed Model
![Sagemaker-Deployed Model](https://github.com/Shashank65536/CloudGroup-12/blob/main/Screenshots/deployed_model.png?raw=true)
###Model Prediction
![Sagemaker-Model Prediction](https://github.com/Shashank65536/CloudGroup-12/blob/main/Screenshots/model_predictions.png?raw=true)
