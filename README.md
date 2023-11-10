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

*The details pertaining to these features are mentioned in the [URL Feature ExtractionLinks.ipynb.]([https://colab.research.google.com/github/shreyagopal/Phishing-Website-Detection-by-Machine-Learning-Techniques/blob/master/URL%20Feature%20Extraction.ipynb](https://colab.research.google.com/drive/1fjDVascByYlb2nQORj1V9fcsTroFD0eb#scrollTo=ybur8dewifEw))*

Together 17 features are extracted from the 10,000 URL dataset and are stored in '[5.urldata.csv](https://github.com/shreyagopal/Phishing-Website-Detection-by-Machine-Learning-Techniques/blob/master/DataFiles/5.urldata.csv)' file in the DataFiles folder.<br>
The features are referenced from the https://archive.ics.uci.edu/ml/datasets/Phishing+Websites.
