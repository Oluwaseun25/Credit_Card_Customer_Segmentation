# Credit Card Customer Segmentation

## Introduction

In this project, we analyze the 'Credit Card Dataset for Clustering' provided by Kaggle to develop customer segmentation using unsupervised learning techniques. This dataset contains usage behavior of about 9000 active credit card holders over a 6-month period. The goal is to identify distinct customer segments to inform marketing strategies.

## Problem Statement

The primary objective is to perform customer segmentation using clustering techniques. We will:
1. Perform hierarchical clustering to identify inherent groupings within the data.
2. Perform partitioning clustering using the K-means algorithm and plot the clusters.
3. Find the optimal number of clusters (k) and plot the clusters again.

For simplicity, we will use only two features: `PURCHASES` and `CREDIT_LIMIT`.

## Dataset Description

The dataset contains the following columns:

- **CUST_ID**: Identification of the credit card holder.
- **BALANCE_FREQUENCY**: How frequently the balance is updated.
- **PURCHASES**: Amount of purchases made from the account.
- **CASH_ADVANCE**: Cash in advance given by the user.
- **CREDIT_LIMIT**: Limit of the credit card for the user.
- **PAYMENTS**: Amount of payment done by the user.

## Clustering Approach

### 1. Hierarchical Clustering
Hierarchical clustering is performed to identify inherent groupings within the data. The dendrogram is used to visualize the clusters and determine an appropriate number of clusters.

### 2. K-means Clustering
K-means clustering is applied to partition the data into distinct clusters. The Elbow method is used to find the optimal value of k. The clusters are then plotted for visualization.

### 3. Optimal K Value
The optimal k value is determined, and the clusters are plotted again to visualize the final segmentation.

## Column Explanation

- **CUST_ID**: Unique identification of the credit card holder.
- **BALANCE_FREQUENCY**: Frequency with which the balance is updated.
- **PURCHASES**: Total amount of purchases made.
- **CASH_ADVANCE**: Cash advance amount given by the user.
- **CREDIT_LIMIT**: Maximum credit limit available on the card.
- **PAYMENTS**: Total payments made by the user.

## K-means Cluster Interpretation

- **Customers in Green**: High spenders making purchases above their credit limit (Extravagant Customers).
- **Customers in Purple**: Average spenders with purchases around their credit limit (Average Spending Customers).
- **Customers in Yellow**: Low spenders with purchases significantly below their credit limit (Cheap Ones).
- **Customers in Blue**: Low spenders with purchases within or below their credit limit (Ambiguous Cluster).
- **Customers in Light Green**: Low spenders staying within their credit limit (Careful Customers).

## Professional Report Based on Findings

### Introduction
Our clustering analysis aimed to identify distinct customer segments based on purchase behavior and credit limits. Through hierarchical and K-means clustering, we uncovered five clusters, each exhibiting unique spending patterns.

### Cluster Insights

#### Extravagant Customers (Green)
- **Characteristics**: High spenders making purchases above their credit limit.
- **Recommendation**: Develop premium credit card offerings with exclusive benefits and rewards to capitalize on their spending potential.
  - Example: Waived or discounted annual fees for maintaining a premium relationship and special loyalty bonuses for card renewal.

#### Average Spending Customers (Purple)
- **Characteristics**: Mix of average purchases above or below their credit limit.
- **Recommendation**: Tailor marketing strategies to provide versatile and flexible credit card options that cater to various spending habits in this segment.

#### Cheap Ones (Yellow)
- **Characteristics**: Customers making low-value purchases significantly below their credit limit.
- **Recommendation**: Design targeted promotions and incentives to attract these customers towards increasing their spending or utilizing additional credit features.

#### Ambiguous Cluster (Blue)
- **Characteristics**: Low-value purchases, both below and within their credit limit.
- **Recommendation**: Further investigation is warranted to understand the specific characteristics of this group. Consider additional features or surveys for a more nuanced interpretation.

#### Careful Customers (Light Green)
- **Characteristics**: Customers making low purchases but staying within their credit limit.
- **Recommendation**: Recognize and reward responsible spending habits. Offer credit education resources and consider promoting credit limit increase opportunities.

## Deployment Using Streamlit

We deploy our clustering model using Streamlit for an interactive web application.

### Installation

To run the Streamlit app, install the necessary libraries:

```sh
pip install pandas matplotlib seaborn scikit-learn
```

### Usage

1. **Clone the repository:**

```sh
git clone https://github.com/Oluwaseun25/Credit_Card_Customer_Segmentation.git
cd Credit_Card_Customer_Segmentation
```

## Conclusion

By performing customer segmentation using hierarchical and K-means clustering, we identified distinct customer segments based on purchase behavior and credit limits. These insights can inform targeted marketing strategies to better cater to the needs of different customer groups.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

We thank Kaggle for providing the dataset and the open-source community for the tools and libraries used in this project.
