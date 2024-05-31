# Customer Segmentation for a Marketing Campaign

## Project Description

This project aims to perform customer segmentation to summarize customer segments for targeted marketing campaigns. The dataset contains various attributes related to customers' demographics, purchase behaviors, and responses to marketing campaigns. The goal is to identify distinct customer segments and profile them based on their characteristics and behaviors.

## Dependencies

To run this project, you will need the following Python libraries:
# Data Manipulation
pandas==1.3.3
numpy==1.21.2

# Data Visualization
matplotlib==3.4.3
plotly==5.3.1
seaborn==0.11.2

# Date and Time Manipulation
datetime==4.3

# Machine Learning
scikit-learn==0.24.2

# Ignore Warnings
warnings==2.0.0


## Dataset

- [Dataset Link](https://www.kaggle.com/datasets/imakash3011/customer-personality-analysis)

### People

- **ID**: Customer's unique identifier
- **Year_Birth**: Customer's birth year
- **Education**: Customer's education level
- **Marital_Status**: Customer's marital status
- **Income**: Customer's yearly household income
- **Kidhome**: Number of children in customer's household
- **Teenhome**: Number of teenagers in customer's household
- **Dt_Customer**: Date of customer's enrollment with the company
- **Recency**: Number of days since customer's last purchase
- **Complain**: 1 if the customer complained in the last 2 years, 0 otherwise

### Products

- **MntWines**: Amount spent on wine in the last 2 years
- **MntFruits**: Amount spent on fruits in the last 2 years
- **MntMeatProducts**: Amount spent on meat in the last 2 years
- **MntFishProducts**: Amount spent on fish in the last 2 years
- **MntSweetProducts**: Amount spent on sweets in the last 2 years
- **MntGoldProds**: Amount spent on gold in the last 2 years

### Promotion

- **NumDealsPurchases**: Number of purchases made with a discount
- **AcceptedCmp1**: 1 if the customer accepted the offer in the 1st campaign, 0 otherwise
- **AcceptedCmp2**: 1 if the customer accepted the offer in the 2nd campaign, 0 otherwise
- **AcceptedCmp3**: 1 if the customer accepted the offer in the 3rd campaign, 0 otherwise
- **AcceptedCmp4**: 1 if the customer accepted the offer in the 4th campaign, 0 otherwise
- **AcceptedCmp5**: 1 if the customer accepted the offer in the 5th campaign, 0 otherwise
- **Response**: 1 if the customer accepted the offer in the last campaign, 0 otherwise

### Place

- **NumWebPurchases**: Number of purchases made through the company’s website
- **NumCatalogPurchases**: Number of purchases made using a catalogue
- **NumStorePurchases**: Number of purchases made directly in stores
- **NumWebVisitsMonth**: Number of visits to the company’s website in the last month

### Target

- Need to perform clustering to summarize customer segments.

## Analysis

### Demographic Analysis

- **Questions**:
  - What is the distribution of customers based on education level, marital status, and income?
- **Visualizations**:
  - Bar charts, pie charts, or histograms for each demographic variable.

### Customer Purchase Behavior

- **Questions**:
  - How much do customers spend on different product categories (e.g., wines, fruits, meats)?
  - Is there a correlation between the amount spent on different product categories?
- **Visualizations**:
  - Box plots, violin plots, or histograms for each product category.
  - Pairwise scatter plots to explore correlations.

### Campaign Response Analysis

- **Questions**:
  - How many customers responded to each campaign?
  - Is there a trend in campaign response over time?
- **Visualizations**:
  - Line chart showing campaign response rates over time.
  - Bar chart showing response rates for each campaign.

### Customer Complaint Analysis

- **Questions**:
  - What proportion of customers have complained in the last 2 years?
  - Is there a relationship between complaints and other customer attributes (e.g., income, education)?
- **Visualizations**:
  - Pie chart or bar chart showing the proportion of customers who complained.
  - Cross-tabulation or heatmap to explore relationships between complaints and other attributes.

### Purchase Channel Preference

- **Questions**:
  - How do customers prefer to make purchases (web, catalog, store)?
- **Visualizations**:
  - Stacked bar chart showing the distribution of purchases across different channels.

### Recency Analysis

- **Questions**:
  - What is the distribution of recency (number of days since the last purchase) among customers?
  - Is there a relationship between recency and other customer attributes or behaviors?
- **Visualizations**:
  - Histogram or density plot showing the distribution of recency.
  - Scatter plot or box plot to explore relationships with other variables.

### Customer Segmentation

- **Questions**:
  - Can we identify distinct customer segments based on their characteristics and behaviors?
- **Visualizations**:
  - Cluster analysis (e.g., using K-means) to identify customer segments.
  - Visualize clusters using scatter plots or parallel coordinate plots.

## Profiling

- **Monetary Status**: Income, total spent.
- **Family Status**: Marital status, kids.
- **Customer Loyalty**: Recency, customer lifetime value, accepted campaigns.
- **Education**
- **Age**
- **Purchase Behavior**

## Findings

**Cluster 0** represents individuals with incomes higher than Clusters 1 and 2 but lower than Cluster 3. They are distributed across age groups, typically in their 40s to 60s. This group tends to purchase more wine and meat products. While they have more complaints than Cluster 3, they still exhibit fewer complaints compared to Cluster 1.

**Cluster 1** represents individuals with the lowest income among the segmented groups. They tend to be less educated and are likely to be in their mid-30s to 40s. Despite having limited financial resources, they exhibit the highest number of complaints, suggesting a heightened sensitivity to product or service quality. This group also engages in fewer purchases and is less likely to participate in loyalty programs.

**Cluster 2** comprises individuals who are likely to have advanced degrees such as PhDs or master's degrees. They have higher incomes compared to Cluster 1 and are typically found in their 40s to 60s. This group is highly likely to have a partner and family. While they exhibit more purchases than Cluster 1, they participate less in loyalty programs and have the lowest number of complaints.

**Cluster 3** consists of individuals with the highest income and spending levels. They exhibit uniform age distribution and are less likely to have a family. This group engages in the highest number of purchases and is actively involved in camps. Despite their high spending, they have fewer complaints compared to Clusters 0 and 1.

## Refrences

- https://medium.com/@soumenatta/customer-segmentation-with-k-means-clustering-5d4c47bad29f
- https://medium.com/@cdanielaam/understanding-affinity-propagation-clustering-hands-on-with-scikit-learn-69406b1cdb1a
- https://www.kaggle.com/code/karnikakapoor/customer-segmentation-clustering
- https://link.springer.com/article/10.1007/s00521-023-09339-6#:~:text=Segment%20profiling%20focuses%20on%20understanding,targeted%20marketing%20efforts%20%5B51%5D.
  
