# Customer Segmentation with K-Means Clustering

A comprehensive data science project that performs customer segmentation analysis on mall customer data using K-Means clustering algorithm. This project identifies distinct customer groups based on demographics and spending behavior to enable targeted marketing strategies.

## 📊 Project Overview

This project analyzes customer data from a mall to segment customers into meaningful groups based on their:
- **Age**
- **Annual Income**
- **Spending Score (1-100)**

The analysis uses K-Means clustering to identify 5 distinct customer segments, each with unique characteristics and recommended marketing strategies.

## 🎯 Key Findings

### Customer Segments Discovered:

| Cluster | Segment Name | Size | Key Characteristics | Marketing Strategy |
|---------|-------------|------|-------------------|-------------------|
| **0** | Pelanggan Hemat | 20 (10%) | Senior customers, low income & spending | Discount promotions, bundling offers |
| **1** | Pelanggan Muda & Potensial | 54 (27%) | Young customers, moderate income, high spending | Social media campaigns, trending products |
| **2** | Pelanggan Premium | 40 (20%) | High income & high spending | Luxury products, VIP services |
| **3** | Rich Konservatif | 39 (19.5%) | High income, very low spending | Quality focus, value education |
| **4** | Pelanggan Standar & Loyal | 47 (23.5%) | Senior customers, moderate income & spending | Customer loyalty programs |

## 🔧 Technologies Used

- **Python 3.x**
- **Pandas** - Data manipulation and analysis
- **NumPy** - Numerical computing
- **Matplotlib & Seaborn** - Static data visualization
- **Plotly** - Interactive visualizations
- **Scikit-learn** - Machine learning algorithms
  - K-Means Clustering
  - StandardScaler & MinMaxScaler
  - Silhouette Score analysis

## 📁 Project Structure

```
├── cluster.ipynb          # Main Jupyter notebook with complete analysis
├── data.csv              # Customer dataset (200 customers)
└── README.md             # Project documentation
```

## 🚀 Getting Started

### Prerequisites

```bash
pip install pandas numpy matplotlib seaborn scikit-learn plotly
```

### Running the Analysis

1. Clone this repository:
```bash
git clone https://github.com/FadilAlfaizii/Clustering.git
cd Clustering
```

2. Open the Jupyter notebook:
```bash
jupyter notebook cluster.ipynb
```

3. Run all cells to reproduce the analysis

## 📈 Analysis Workflow

### 1. Data Loading & Exploration
- Load customer dataset (200 customers, 5 features)
- Perform basic data exploration and visualization
- Analyze distributions of age, income, and spending patterns

### 2. Data Preprocessing
- Handle missing values (none found)
- Apply data normalization using StandardScaler
- Prepare features for clustering

### 3. Optimal Cluster Selection
- **Elbow Method**: Identify the optimal number of clusters
- **Silhouette Analysis**: Validate cluster quality
- **Result**: K=5 clusters chosen based on clear elbow point and high silhouette score (0.417)

### 4. K-Means Clustering
- Apply K-Means algorithm with k=5
- Generate cluster labels for all customers
- Achieve final silhouette score of 0.417

### 5. Cluster Analysis & Profiling
- Analyze demographic and behavioral characteristics of each cluster
- Create detailed customer personas
- Develop targeted marketing strategies

### 6. Visualization & Insights
- Interactive 2D and 3D scatter plots
- Distribution analysis by cluster
- Statistical profiling of customer segments

## 📊 Dataset Information

- **Source**: Mall Customer Data
- **Size**: 200 customers
- **Features**:
  - CustomerID: Unique identifier
  - Gender: Male/Female
  - Age: Customer age in years
  - Annual Income (k$): Annual income in thousands of dollars
  - Spending Score (1-100): Score assigned based on customer behavior and spending nature

## 🎨 Key Visualizations

The project includes comprehensive visualizations:
- Age, income, and spending score distributions
- Gender distribution analysis
- Interactive 2D clustering visualization (Income vs Spending Score)
- 3D cluster visualization with all three features
- Cluster profiling charts and comparisons

## 💡 Business Recommendations

### Marketing Strategies by Segment:

1. **Pelanggan Premium (20%)**: Focus on luxury products, VIP services, and exclusive experiences
2. **Pelanggan Muda & Potensial (27%)**: Leverage social media marketing and trend-based products
3. **Rich Konservatif (19.5%)**: Emphasize product quality, durability, and long-term value
4. **Pelanggan Standar & Loyal (23.5%)**: Maintain loyalty through consistent service and relevant products
5. **Pelanggan Hemat (10%)**: Target with discounts, sales, and value bundles

## 📈 Model Performance

- **Final Silhouette Score**: 0.417 (indicating good cluster separation)
- **Clusters**: 5 distinct segments
- **Data Coverage**: 100% of customers successfully segmented

## 🤝 Contributing

Feel free to fork this project and submit pull requests for any improvements:
1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 👨‍💻 Author

**Fadil Alfaizi**
- GitHub: [@FadilAlfaizii](https://github.com/FadilAlfaizii)

## 🙏 Acknowledgments

- Dataset source: Mall Customer Segmentation Data
- Inspiration from various customer analytics and segmentation studies
- Thanks to the open-source community for the amazing tools and libraries

---

*This project demonstrates the application of unsupervised machine learning techniques for business intelligence and customer analytics.*
