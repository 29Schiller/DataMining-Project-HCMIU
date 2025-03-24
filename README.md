<div id="top" align="center">
</div>
<!-- PROJECT LOGO -->
<div align="center">
<h1 align="center">Data Mining Project</h1>
  <h3 align="center">
    Applying nine classification algorithms for evaluating the efficiency on the Airline Passenger Satisfaction Dataset
    <br />
    <br />
    <a href="https://github.com/dngcphngnh04/DataMining-Project/issues">Report Bug</a>
    ·
    <a href="https://github.com/dngcphngnh04/DataMining-Project/issues">Request Feature</a>
  </h3>

[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Issues][issues-shield]][issues-url]

</div>

# ABOUT

## 1. The team behind it

| No. |       Full Name        | Student's ID |              Email               |                  Github account                   |                               Roles                                |
| :-: | :--------------------: | :----------: | :------------------------------: | :-----------------------------------------------: | :----------------------------------------------------------------: |
|  1  | Dương Ngọc Phương Anh | ITDSIU22135  | ITDSIU22135@student.hcmiu.edu.vn |     [dngcphngnh04](https://github.com/dngcphngnh04)     |   **TEAM LEADER** with Model evaluation, Hyper-parameters tuning   |
|  2  | Nguyễn Minh Đạt | ITDSIU22166  | ITDSIU22166@student.hcmiu.edu.vn |    [29Schiller](https://github.com/29Schiller)    |              Data preprocessing, Optimize performance              |
|  3  | Nguyễn Hải Phú | ITDSIU22179  | ITDSIU22179@student.hcmiu.edu.vn |     [haiphu241](https://github.com/haiphu241)     | Implement classification/prediction algorithms in Java, Bug fixing |


## 2. The project we are working on

The primary goal of this project is to evaluate the effectiveness, accuracy, and relevance of these machine learning models in addressing classification problems, particularly in predicting survival outcomes.


## 3. Goal
The purpose of this project is to develop an advanced data mining framework composed of two key components, each designed to address specific analytical objectives and provide valuable insights:
-	The first component is a classification and prediction model that integrates the strengths of Decision Trees, Naive Bayes, and IBK algorithms. This model will leverage key features such as demographic attributes, ticket class, and other relevant variables to accurately predict passenger survival. By combining these algorithms, the framework ensures a balanced approach, utilizing Decision Trees for their interpretability, Naive Bayes for its probabilistic predictions, and IBK for its adaptability to instance-based learning. Together, these methods aim to deliver robust and reliable predictions.
-	The second component is a sequence mining algorithm, which seeks to uncover hidden sequential patterns within the dataset. This algorithm will identify logical relationships and temporal dependencies between events, providing a deeper understanding of how different factors interact over time to influence survival outcomes. By analyzing these patterns, the framework will reveal meaningful insights that go beyond static feature relationships.


# REASON

## 1. Motivation

Airplane passenger satisfaction has become a critical focus for airlines aiming to enhance customer experience and maintain competitive advantage. Factors influencing satisfaction range from tangible elements like seat comfort, food quality, and punctuality to intangible aspects such as service quality, staff behavior, and ease of communication. With the rapid advancement of technology, airlines have introduced features like in-flight entertainment, Wi-Fi connectivity, and streamlined check-in processes to improve customer experience. This data mining project seeks to analyze passenger satisfaction by leveraging a classification model to identify the key determinants that contribute to a positive travel experience. By uncovering these insights, airlines can implement targeted strategies to elevate service standards and address common pain points, ensuring higher customer retention and loyalty.
## 2. Idea
This study examines airplane passenger satisfaction using data mining techniques to uncover key determinants of a positive flying experience. It evaluates the accuracy of machine learning algorithms in predicting satisfaction levels and explores their practical applications in improving airline services. By identifying critical factors, the research aims to help airlines enhance customer experiences, increase loyalty, and optimize service offerings.




## 3. Roadmap

- [x] Data collecting
- [x] Data pre-processing
- [x] Build model to classify

Please see the [open issues](https://github.com/dngcphngnh04/DataMining-Project/issues) for a full list of proposed features (
and known issues).

# METHODOLOGY (based on theory class)

## 1. Ask a question

This study focuses on analyzing airplane passenger satisfaction using data mining techniques. It investigates the effectiveness of machine learning algorithms in identifying factors that influence satisfaction and their practical implications for improving customer experience. The research aims to help airlines enhance service quality, boost customer retention, and ensure a more enjoyable travel experience for passengers.



## 2. Data gathering

This study examines airplane passenger satisfaction using data mining techniques to uncover key determinants of a positive flying experience. It evaluates the accuracy of machine learning algorithms in predicting satisfaction levels and explores their practical applications in improving airline services. By identifying critical factors, the research aims to help airlines enhance customer experiences, increase loyalty, and optimize service offerings.



## 3. Data cleaning

The pre-processing stage of a depression study involved categorizing responses into five groups based on depression-related factors. Python's'shuffle' function ensured no inherent order or bias. Python was used for data processing due to Weka's limitations and Java's difficulties. Missing data was filled using an imputation method, and string-type responses were converted into numerical form using label encoding. The original dataset had long column names, requiring special encoding for quick access. Questions were encoded with alphabetical letters for clarity. This pre-processing made the dataset suitable for further analysis and machine learning methods.

## 4. Model building

Machine learning algorithms are crucial for creating classification models, as they identify trends and make data-driven judgments. Techniques like ibk, J48, Logistic Regression, Naive Bayes, OneR, SVM, AdaBoostM1, RandomForest are used to classify instances based on their closest neighbors, making them suitable for pattern recognition tasks, binary classification, and large datasets. Ensemble approaches like AdaBoostM1 and RandomForest increase classification performance by integrating multiple classifiers. Weka supports these models and offers full modeling and training capabilities, making the development process easier. Weka functions like buildClassifier are often used throughout the model development process, making the training process quick for many classifiers.

## 5. Return the result

The final step involves evaluating a machine learning model on a test dataset to assess its effectiveness in identifying and forecasting depression levels. This evaluation uses measures like accuracy, precision, recall, and F1 score, ensuring the model's dependability, accuracy, and generalization capabilities. This step is crucial for enabling proactive early depression detection and management, enhancing student well-being. The model's efficacy is assessed using functions like toSummaryString, toMatrixString, and metrics, providing comprehensive results for a comprehensive study.

# PROJECT STRUCTURE

- `.idea` folder: provides project-specific parameters and configurations for IntelliJ IDEA
- `Data` folder: to hold the datasets organized by family, love, self, study, and job subfolders. Each contains the full training, testing, and validation dataset in both CSV and ARFF format supported by the Weka
- `Evaluation Result + Report` folder: it contains the Evaluation results produced in CSV format and our Report for the Data Mining Project
- `Colab Notebook` folder: the folder contains the Colab Notebook for the Preprocessing Stage of the dataset.
- `lib` folder: contains external libraries and dependencies needed for the project (weka.jar)
- `out` folder: stores compiled output files, such as class files
- `src` folder: the primary source directory for the project’s code
  - `BaseModel` subfolder:
    - `ModelPre_Tuning` subfolder: provides foundational classifier Java classes for this project. That includes IBk, J48, Logistic Regression, Naïve Bayes, OneR, SVM  and ZeroR as default.
    - `TuningModel` subfolder: provides foundational classifier Java classes for this project. That includes IBk, J48, Logistic Regression, OneR and SVM as tuning models.
  - `EnsembleModel` subfolder:
    - `ModelPre_Tuning` subfolder: contains the ensemble model classes that incorporate many classifiers. That includes AdaBoostM1, and RandomForest as default.
    - `TuningModel` subfolder: contains the ensemble model classes that incorporate many classifiers. That includes AdaBoostM1, and RandomForest as tuning models.
  - `Preprocessing` folder:
    - `AttributeSelection.java`: class to import data from the specified path
    - `CSV2Arff.java`: the class for processing and preparing data
    - `DataPreprocess.java`: class to enable feature selection algorithms
- `README.md`: a document to outline and explain the project

# CONTACT

Project Link: **[GitHub HERE](https://github.com/dngcphngnh04/DataMining-Project)**

<!-- ACKNOWLEDGMENTS -->

# ACKNOWLEDGEMENTS

We want to express our sincerest thanks to our lecturer and the people who have helped us to achieve this project's
goals:

- []() Dr. Nguyen Thi Thanh Sang
- []() MSc. Nguyen Quang Phu
- []() The README.md template from **[othneildrew](https://github.com/othneildrew/Best-README-Template)**


<!-- MARKDOWN LINKS & IMAGES -->

[contributors-shield]: https://img.shields.io/github/contributors/dngcphngnh04/DataMining-Project.svg?style=for-the-badge
[contributors-url]: https://github.com/dngcphngnh04/DataMining-Project/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/dngcphngnh04/DataMining-ProjectC.svg?style=for-the-badge
[forks-url]: https://github.com/dngcphngnh04/DataMining-Project/network/members
[issues-shield]: https://img.shields.io/github/issues/dngcphngnh04/DataMining-Project.svg?style=for-the-badge
[issues-url]: https://github.com/dngcphngnh04/DataMining-Project/issues
