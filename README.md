# Phishing-Website-Detection
A phishing website is a common social engineering method that mimics trustful uniform resource locators (URLs) and webpages

## **1. Objective:**
A phishing website is a common social engineering method that mimics trustful uniform resource locators (URLs) and webpages. The objective of this project is to train machine learning models and deep neural nets on the dataset created to predict phishing websites. Both phishing and benign URLs of websites are gathered to form a dataset and from them required URL and website content-based features are extracted. The performance level of each model is measures and compared.

*This project is worked on Google Collaboratory.*<br>
*The required packages for this notebook are imported when needed.*

## **2. Loading Data:**

The features are extracted and store in the csv file. The working of this can be seen in the 'Phishing Website Detection_Feature Extraction.ipynb' file.

The reulted csv file is uploaded to this notebook and stored in the dataframe.

## **3. Familiarizing with Data**
In this step, few dataframe methods are used to look into the data and its features.

## **4. Visualizing the data**
Few plots and graphs are displayed to find how the data is distributed and the how features are related to each other.
![image](https://github.com/Mugeshcybersecurity/Phishing-Website-Detection/assets/95292025/607d5bd7-011d-42ad-81ac-214f9695867d)

![image](https://github.com/Mugeshcybersecurity/Phishing-Website-Detection/assets/95292025/86733b54-6587-4427-88ef-2110410ed5a7)

## **5. Data Preprocessing & EDA**
Here, we clean the data by applying data preprocesssing techniques and transform the data to use it in the models.

|   | Have_IP |      Have_At |   URL_Length |    URL_Depth |  Redirection | https_Domain |      TinyURL | Prefix/Suffix |   DNS_Record |  Web_Traffic |   Domain_Age |   Domain_End |     iFrame |   Mouse_Over | Right_Click | Web_Forwards |        Label |              |
|---|--------:|-------------:|-------------:|-------------:|-------------:|-------------:|-------------:|--------------:|-------------:|-------------:|-------------:|-------------:|-----------:|-------------:|------------:|-------------:|-------------:|--------------|
|   |  count  | 10000.000000 | 10000.000000 | 10000.000000 | 10000.000000 | 10000.000000 | 10000.000000 |  10000.000000 | 10000.000000 | 10000.000000 | 10000.000000 | 10000.000000 | 10000.0000 | 10000.000000 | 10000.00000 |  10000.00000 | 10000.000000 | 10000.000000 |
|   |   mean  |     0.005500 |     0.022600 |     0.773400 |     3.072000 |     0.013500 |     0.000200 |      0.090300 |     0.093200 |     0.100800 |     0.845700 |     0.413700 |     0.8099 |     0.090900 |     0.06660 |      0.99930 |     0.105300 |     0.500000 |
|   |   std   |     0.073961 |     0.148632 |     0.418653 |     2.128631 |     0.115408 |     0.014141 |      0.286625 |     0.290727 |     0.301079 |     0.361254 |     0.492521 |     0.3924 |     0.287481 |     0.24934 |      0.02645 |     0.306955 |     0.500025 |
|   |   min   |     0.000000 |     0.000000 |     0.000000 |     0.000000 |     0.000000 |     0.000000 |      0.000000 |     0.000000 |     0.000000 |     0.000000 |     0.000000 |     0.0000 |     0.000000 |     0.00000 |      0.00000 |     0.000000 |     0.000000 |
|   |   25%   |     0.000000 |     0.000000 |     1.000000 |     2.000000 |     0.000000 |     0.000000 |      0.000000 |     0.000000 |     0.000000 |     1.000000 |     0.000000 |     1.0000 |     0.000000 |     0.00000 |      1.00000 |     0.000000 |     0.000000 |
|   |   50%   |     0.000000 |     0.000000 |     1.000000 |     3.000000 |     0.000000 |     0.000000 |      0.000000 |     0.000000 |     0.000000 |     1.000000 |     0.000000 |     1.0000 |     0.000000 |     0.00000 |      1.00000 |     0.000000 |     0.500000 |
|   |   75%   |     0.000000 |     0.000000 |     1.000000 |     4.000000 |     0.000000 |     0.000000 |      0.000000 |     0.000000 |     0.000000 |     1.000000 |     1.000000 |     1.0000 |     0.000000 |     0.00000 |      1.00000 |     0.000000 |     1.000000 |
|   |   max   |     1.000000 |     1.000000 |     1.000000 |    20.000000 |     1.000000 |     1.000000 |      1.000000 |     1.000000 |     1.000000 |     1.000000 |     1.000000 |     1.0000 |     1.000000 |     1.00000 |      1.00000 |     1.000000 |     1.000000 |

## **7. Machine Learning Models & Training**

From the dataset above, it is clear that this is a supervised machine learning task. There are two major types of supervised machine learning problems, called classification and regression. 

This data set comes under classification problem, as the input URL is classified as phishing (1) or legitimate (0). The supervised machine learning models (classification) considered to train the dataset in this notebook are:
* Decision Tree
* Random Forest
* Multilayer Perceptrons
* XGBoost
* Autoencoder Neural Network
* Support Vector Machines


## **8. Comparision of Models**
To compare the models performance, a dataframe is created. The columns of this dataframe are the lists created to store the results of the model.

