# Customer Segmentation using KMeans and PCA

This project performs customer segmentation based on online transaction data using clustering techniques, dimensionality reduction, and visualization.

## Dataset

The dataset used is `int_online_tx.csv`, which contains transaction records including:
- `CustomerID`
- `InvoiceNo`
- `StockCode`
- `Quantity`
- `UnitPrice`

## Objectives

- Clean and preprocess the transaction data.
- Engineer features representing customer behavior.
- Standardize the data for modeling.
- Apply PCA to reduce dimensionality.
- Perform clustering using KMeans.
- Visualize the customer segments and key statistics.

## Steps

1. **Data Cleaning**: Remove missing `CustomerID` values and create a `Sales` column.
2. **Feature Engineering**: Aggregate features like total transactions, products bought, total sales, and quantities.
3. **Standardization**: Normalize features using `StandardScaler`.
4. **Dimensionality Reduction**: Apply PCA to reduce to 2 principal components.
5. **Clustering**: Use KMeans with 4 clusters.
6. **Visualization**:
   - PCA Scatterplot of clusters.
   - Boxplot of total sales by cluster.
   - Count plot of customers in each cluster.
   - Correlation heatmap of engineered features.

## Requirements

- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

Install requirements using:

```bash
pip install -r requirements.txt
