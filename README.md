# Simulated Customer Clustering Analysis

## Project Overview

This project implements comprehensive customer segmentation and clustering analysis using machine learning techniques to identify customer behavior patterns and provide data-driven insights for sales and marketing strategies.

## Objectives

- **Customer Segmentation**: Group customers using advanced clustering algorithms
- **Behavior Analysis**: Identify characteristics and patterns of different customer segments  
- **Strategic Insights**: Provide actionable insights for sales and marketing teams
- **Value Optimization**: Identify high-value customer segments for targeted strategies
- **Retention Enhancement**: Improve customer retention rates and satisfaction

## Key Features

### RFM Analysis
- **Recency**: Days since last purchase
- **Frequency**: Number of unique transactions per quarter
- **Monetary**: Total spending amount and average order value

### Advanced Customer Features
- **Customer Lifetime**: Total quarters from first to last purchase
- **Geographic Segmentation**: Analysis by billing country
- **Churn Risk**: Binary indicator for customers inactive >365 days
- **Product Diversification**: Number of unique products purchased
- **Big Order Analysis**: High-value order patterns

### Machine Learning Implementation
- **K-Means Clustering**: Primary segmentation algorithm
- **Hierarchical Clustering**: Alternative clustering approach
- **Feature Engineering**: Log transformations and scaling
- **Customer Status Classification**: New, Existing, Churn categorization

## Technical Stack

### Core Libraries
```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
from sklearn.cluster import KMeans
from sklearn.preprocessing import StandardScaler
from scipy.cluster.hierarchy import dendrogram, linkage, fcluster
```

### Data Processing
- **Pandas**: Data manipulation and analysis
- **NumPy**: Numerical computations
- **Scikit-learn**: Machine learning algorithms and preprocessing

### Visualization
- **Matplotlib**: Statistical plotting
- **Seaborn**: Advanced statistical visualizations

## Project Structure

```
simulated_customer_clustering/
├── simulated_clustering.ipynb           # Main analysis notebook
├── sales_order_simulated_v13.csv        # Primary dataset
├── sales_order_simulated_v7p6.csv       # Alternative dataset
├── customer_analysis_by_cluster_simulated.xlsx  # Results analysis
└── README.md                            # This documentation
```

## Key Analysis Components

### 1. Data Preprocessing
- Data cleaning and validation
- Feature engineering and transformation
- Missing value handling
- Date parsing and period calculations

### 2. Customer Feature Engineering
- RFM metrics calculation
- Customer lifetime analysis
- Geographic and product diversification metrics
- Churn risk assessment

### 3. Clustering Analysis
- K-means clustering implementation
- Optimal cluster number determination
- Hierarchical clustering comparison
- Cluster validation and interpretation

### 4. Business Intelligence
- Customer segment profiling
- High-value customer identification
- Churn risk analysis
- Geographic distribution insights

## Getting Started

### Prerequisites
```bash
pip install pandas numpy matplotlib seaborn scikit-learn scipy openpyxl
```

### Running the Analysis
1. Open Jupyter Notebook
2. Navigate to the project directory
3. Open `simulated_clustering.ipynb`
4. Run all cells sequentially

### Input Data Format
The analysis expects CSV files with the following columns:
- `Customer_Group`: Unique customer identifier
- `Date`: Transaction date
- `Amount`: Transaction amount
- `Doc_No`: Document/order number
- `Billing_Country`: Customer location
- `Broad_Phase`: Product category
- `Material_Name`: Product details

## Analysis Outputs

### Customer Segments
- **High-Value Customers**: Premium segment with high monetary value
- **Loyal Customers**: Regular purchasers with consistent behavior
- **New Customers**: Recent additions to customer base
- **At-Risk Customers**: Showing signs of potential churn

### Key Metrics
- Customer lifetime value calculation
- Churn probability scoring
- Geographic distribution analysis
- Product preference patterns

### Visualization Outputs
- Cluster scatter plots
- Customer distribution charts
- RFM analysis heatmaps
- Geographic performance maps

## Business Applications

### Sales Team Benefits
- **Customer Prioritization**: Focus on high-value segments
- **Targeted Strategies**: Customize approach by customer type
- **Performance Tracking**: Monitor customer journey progression

### Marketing Team Benefits
- **Personalized Campaigns**: Segment-specific messaging
- **Resource Allocation**: Optimize marketing spend
- **Retention Programs**: Proactive churn prevention

### Management Insights
- **Strategic Planning**: Data-driven customer strategy
- **Risk Management**: Early churn detection
- **Growth Opportunities**: Identify expansion potential

## Technical Implementation Details

### Clustering Algorithm
- **K-Means**: Primary clustering method with optimal k determination
- **Preprocessing**: StandardScaler for feature normalization
- **Validation**: Silhouette analysis and elbow method

### Feature Engineering
- **Log Transformations**: Handle skewed distributions
- **Categorical Encoding**: Geographic and product features
- **Temporal Features**: Quarterly and lifetime calculations

### Performance Metrics
- **Cluster Cohesion**: Within-cluster sum of squares
- **Separation**: Between-cluster distances
- **Business Validation**: Segment profitability analysis

## Results and Insights

The analysis provides actionable insights for:
- Customer retention strategies
- Revenue optimization opportunities
- Market expansion planning
- Risk mitigation approaches

## Future Enhancements

### Potential Improvements
- **Real-time Scoring**: Live customer risk assessment
- **Predictive Modeling**: Churn prediction algorithms
- **Advanced Segmentation**: Multi-dimensional clustering
- **Dashboard Integration**: Interactive visualization tools

### Model Extensions
- **Time Series Analysis**: Seasonal pattern detection
- **Collaborative Filtering**: Product recommendation engine
- **Survival Analysis**: Customer lifetime modeling

## Contributing

To contribute to this project:
1. Review the analysis methodology
2. Suggest feature improvements
3. Validate business insights
4. Enhance visualization capabilities

## Contact and Support

For questions or support regarding this analysis:
- Review the notebook documentation
- Check the output Excel files for detailed results
- Refer to the clustering validation metrics

---

**Note**: This analysis uses simulated data for demonstration purposes. Real-world implementation should include additional validation and business context consideration.