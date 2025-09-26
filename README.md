# Simulated Customer Clustering Analysis

## Project Overview

This project implements comprehensive customer segmentation and clustering analysis using machine learning techniques including PCA, t-SNE, and multiple clustering algorithms to identify customer behavior patterns and provide data-driven insights for sales and marketing strategies.

## Objectives

- **Multi-Method Customer Segmentation**: Group customers using K-means, hierarchical clustering, and dimensionality reduction techniques
- **Behavior Analysis**: Identify characteristics and patterns using PCA and t-SNE visualization
- **Comparative Model Evaluation**: Compare clustering performance across different methodologies
- **Strategic Insights**: Provide actionable insights for sales and marketing teams through advanced analytics
- **Value Optimization**: Identify high-value customer segments for targeted strategies
- **Retention Enhancement**: Improve customer retention rates and satisfaction through data-driven segmentation

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
- **K-Means Clustering**: Primary segmentation algorithm with elbow method and silhouette analysis
- **Hierarchical Clustering**: Alternative clustering approach with dendrogram analysis
- **PCA (Principal Component Analysis)**: Dimensionality reduction for feature optimization
- **t-SNE (t-Distributed Stochastic Neighbor Embedding)**: Advanced visualization for cluster validation
- **Feature Engineering**: Log transformations, standardization, and scaling
- **Model Comparison**: Comparative analysis between PCA-based and original feature clustering
- **Customer Status Classification**: New, Existing, Churn categorization



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

### 3. Advanced Clustering Analysis
- **K-means clustering**: Implementation with elbow method and silhouette analysis
- **PCA-based clustering**: Dimensionality reduction to capture 90% variance
- **Hierarchical clustering**: Dendrogram analysis and alternative segmentation
- **t-SNE visualization**: Non-linear visualization for cluster validation
- **Comparative analysis**: Performance comparison between different clustering approaches
- **Optimal cluster determination**: Multiple validation metrics and visualization techniques

### 4. Business Intelligence
- Customer segment profiling
- High-value customer identification
- Churn risk analysis
- Geographic distribution insights





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
- **PCA Analysis**: Scree plots and cumulative variance charts
- **Cluster Comparison**: Side-by-side analysis of PCA vs original feature clustering
- **t-SNE Visualizations**: Non-linear 2D representations of customer segments
- **Silhouette Analysis**: Cluster quality evaluation and comparison
- **Hierarchical Dendrograms**: Tree-based cluster structure visualization
- **Multi-panel Dashboards**: Comprehensive comparative analysis charts
- **RFM Heatmaps**: Cluster characteristics analysis
- **Geographic Distribution**: Customer location-based insights

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

### Clustering Algorithms
- **K-Means**: Primary clustering method with optimal k determination using elbow method
- **Hierarchical Clustering**: Ward linkage with dendrogram analysis
- **PCA Integration**: Dimensionality reduction clustering for variance optimization
- **Preprocessing**: StandardScaler for feature normalization across all methods
- **Validation**: Comprehensive silhouette analysis and comparative metrics

### Feature Engineering
- **Log Transformations**: Handle skewed distributions
- **Categorical Encoding**: Geographic and product features
- **Temporal Features**: Quarterly and lifetime calculations

### Performance Metrics
- **Silhouette Analysis**: Cluster quality measurement across all methods
- **Elbow Method**: Optimal cluster number determination
- **Variance Explained**: PCA component contribution analysis  
- **Inertia Comparison**: Within-cluster sum of squares across methods
- **Cross-Method Validation**: Performance comparison between PCA and original feature clustering
- **Business Validation**: Segment profitability and behavioral analysis

## Results and Insights

The comprehensive multi-method analysis provides actionable insights for:
- **Method Comparison**: Comparative evaluation shows performance differences between PCA-based and original feature clustering
- **Customer Retention**: Data-driven strategies based on advanced segmentation techniques
- **Revenue Optimization**: High-value segment identification through multiple clustering approaches
- **Market Expansion**: Geographic and behavioral pattern analysis
- **Risk Mitigation**: Advanced churn prediction through hierarchical and K-means analysis
- **Cluster Validation**: t-SNE visualization confirms meaningful customer segment separation

## Future Enhancements

### Potential Improvements
- **Real-time Scoring**: Live customer risk assessment with automated model updates
- **Advanced Ensemble Methods**: Combining multiple clustering approaches for robust segmentation
- **Deep Learning Integration**: Neural network-based customer representation learning
- **Interactive Dashboards**: Real-time visualization tools with drill-down capabilities
- **UMAP Visualization**: Alternative to t-SNE for better preservation of global structure

### Model Extensions
- **Time Series Analysis**: Seasonal pattern detection and temporal clustering
- **Collaborative Filtering**: Product recommendation engine based on cluster behavior
- **Survival Analysis**: Customer lifetime modeling with advanced statistical methods
- **Multi-dimensional Scaling**: Additional dimensionality reduction techniques
- **Ensemble Clustering**: Consensus clustering across multiple algorithms

## Contributing

To contribute to this project:
1. **Review Methodology**: Analyze the multi-method clustering approach and validation techniques
2. **Algorithm Improvements**: Suggest enhancements to PCA, t-SNE, or clustering implementations
3. **Validation Enhancement**: Improve cluster validation and business metric alignment
4. **Visualization Development**: Enhance advanced visualization capabilities and interactive features
5. **Performance Optimization**: Optimize computational efficiency for large datasets

## Contact and Support

For questions or support regarding this analysis:
- **Methodology Questions**: Review the comprehensive notebook documentation covering PCA, t-SNE, and clustering comparisons
- **Technical Implementation**: Check the advanced scikit-learn implementations and model validation sections
- **Results Analysis**: Refer to the output Excel files for detailed cluster characteristics and performance metrics
- **Business Applications**: Review the cluster validation sections for business insight interpretation

---

**Note**: This analysis uses simulated data for demonstration purposes and implements advanced machine learning techniques. Real-world implementation should include additional validation, business context consideration, and may require computational optimization for large-scale datasets.