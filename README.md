# Phishing-Website-Detection-by-Machine-Learning-Techniques

# Data Collection

The collection of phishing URLs is sourced from the open-source service PhishTank, which provides a variety of phishing URLs in formats such as CSV and JSON. This service is regularly updated on an hourly basis.

To download the data: [PhishTank Developer Info](https://www.phishtank.com/developer_info.php)

From this dataset, 5000 random phishing URLs are selected for training the machine learning models.

Legitimate URLs are obtained from the open datasets provided by the University of New Brunswick, available at https://www.unb.ca/cic/datasets/url-2016.html. This dataset encompasses benign, spam, phishing, malware, and defacement URLs. For this project, the dataset containing benign URLs is chosen. 5000 random legitimate URLs are then selected from this dataset for training the machine learning models.

The datasets mentioned above are uploaded to the [DataFiles Folder](./DataFiles)
folder within this repository.

## Feature Extraction
The below-mentioned category of features are extracted from the URL data:

1.   Address Bar-based Features <br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;In this category 9 features are extracted.
2.   Domain-based Features<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;In this category 4 features are extracted.
3.   HTML & Javascript based Features<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;In this category 4 features are extracted.

*The details pertaining to these features are mentioned here  [DataFiles Folder](./DataFiles/URL_Feature_Extraction.ipynb)


Together 17 features are extracted from the 10,000 URL dataset and are stored in [5.urldata.csv](./DataFiles/5.urldata.csv)

## Machine learning models and Training

The dataset is treated as a classification problem, distinguishing between phishing and legitimate URLs. Various supervised machine learning models are considered for training. <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;In          Decision Tree <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;In          Random Forest <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;In         Multilayer Perceptrons <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;In          XGBoost <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;In          Autoencoder Neural Network <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;In          Support Vector Machines <be>

All these models are trained using the dataset, and the evaluation of each model is conducted using the test dataset and can be found here- [Model Trained](./Train_models_Phishing_Website_Detection.ipynb)


## Presentation [Click here to see presentation](./Presentation.pptx)

