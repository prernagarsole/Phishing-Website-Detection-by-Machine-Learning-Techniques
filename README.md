# Phishing-Website-Detection-by-Machine-Learning-Techniques

**Data Collection**

The collection of phishing URLs is sourced from the open-source service PhishTank, which provides a variety of phishing URLs in formats such as CSV and JSON. This service is regularly updated on an hourly basis.

To download the data: [PhishTank Developer Info](https://www.phishtank.com/developer_info.php)

From this dataset, 5000 random phishing URLs are selected for training the machine learning models.

Legitimate URLs are obtained from the open datasets provided by the University of New Brunswick, available at https://www.unb.ca/cic/datasets/url-2016.html. This dataset encompasses benign, spam, phishing, malware, and defacement URLs. For this project, the dataset containing benign URLs is chosen. 5000 random legitimate URLs are then selected from this dataset for training the machine learning models.

The datasets mentioned above are uploaded to the [DataFiles Folder](./DataFiles)
folder within this repository.
