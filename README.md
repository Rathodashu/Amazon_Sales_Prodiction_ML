## Project Explanation:## 
This project is an analysis of Amazon Sales Data that covers various regions, countries, and sales channels. 
The aim is to extract insights, perform exploratory data analysis (EDA), and apply clustering techniques for better customer segmentation based on sales and profits. 
The steps are organized into several sections as follows:

### Data Understanding and Cleaning:

The dataset is loaded using pandas, followed by an initial inspection using functions like .head(), .tail(), and .info().
Missing values are identified, and columns like 'Order Date' are converted into datetime format for easier manipulation. 
Additionally, the year and month are extracted from the 'Order Date' column for temporal analysis.

### Basic Data Analysis:

The number of unique regions, countries, item types, and other categorical data are calculated.
The total units sold, unit cost, total revenue, total cost, and total profit are also computed. This gives a high-level overview of the dataset's sales and financial performance.

### Region and Sales Channel Analysis:

The dataset is grouped by Region and Sales Channel to understand how profits vary across these dimensions.
Insights reveal regional preferences in sales channels, such as:
Sub-Saharan Africa has strong offline sales.
Europe shows a balance between online and offline channels.
Asia and Australia have competitive online channels.

### Exploratory Data Analysis (EDA):

Various visualizations are created using Seaborn and Matplotlib to uncover trends in the data:
Bar charts show yearly sales performance.
Pie charts and donut charts highlight region-wise unit sales, revenue distribution across regions, and sales channels.
The sales performance of different item types is visualized through bar charts, and sales channel revenue distribution is shown with pie charts.

### Clustering and Model Selection:

The K-Means clustering algorithm is applied to segment the data based on the Units Sold and Total Profit.
Different values of K (number of clusters) are tested using the Elbow Method to determine the optimal number of clusters.
The data is clustered into 3 groups, and the clusters are visualized. Centroids are plotted to represent the central point of each cluster.
The clusters are analyzed in terms of their mean values, and item types are examined within each cluster.
A Silhouette Score is calculated to evaluate the quality of the clusters, indicating how well-separated the clusters are.
