# Mail-order Customer Segmentation and Prediction

This project aims to help a mail-order sales company identify potential customers in the general population by applying customer segmentation and supervised learning techniques. The project has two main parts:

1. **Unsupervised Learning: Customer Segmentation** - Analyze demographics data for the general population and the company's existing customers to discover segments of the population that are more likely to be customers of the company.
2. **Supervised Learning: Predictive Model** - Build a machine learning model to predict whether an individual from the general population will become a customer based on their demographic information.

## Table of Contents

- [Data](#data)
- [Requirements](#requirements)
- [Instructions](#instructions)
- [Methodology](#methodology)
- [Results](#results)
- [License](#license)


## Data

The data used in this project was provided by Bertelsmann Arvato Analytics, and represents a real-life data science task. The data includes:

- General population demographics
- Customers demographics
- Mailout campaign data

Due to the terms of use, the data is not publicly available and therefore not included in this repository.

## Requirements

Python 3.6 or above is required to run the code in this repository. All required packages can be installed by running:

```bash
pip install -r requirements.txt
```

## Instructions

1. Clone the repository and navigate to the downloaded folder.
```bash
git clone https://github.com/<username>/<repository>.git
cd <repository>
```

2. Install required Python packages.
```bash
pip install -r requirements.txt
```

3. Run the Jupyter notebook.
```bash
jupyter notebook <notebook_name>.ipynb
```

4. Follow the instructions in the notebook.

## Methodology

The project is divided into two major parts:

1. **Customer Segmentation Report:** This part involved unsupervised learning techniques, PCA and k-means clustering, to perform customer segmentation, identifying the core customer traits from a demographics data.

2. **Supervised Learning Model:** With the knowledge of who our core customer is, we used a machine learning classification model to predict whether or not each individual in the mailout campaign would convert into becoming a customer. The model was selected and tuned using GridSearchCV and evaluated based on the ROC AUC score due to the imbalanced nature of the response variable.

## Results

- We identified specific segments of the population that are more likely to be customers of the company by applying clustering techniques on the demographics data.
- A supervised learning model (XGBoost) was built to predict whether an individual from the general population will become a customer based on their demographic information. The model achieved a good performance on the training set but tended to predict all the labels negative due to the imbalanced classes.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
