# Mental Health Analysis in Tech Industry

## Unsupervised Machine Learning Project

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

---

## 📋 Project Overview

This project analyzes mental health trends in the technology industry using unsupervised machine learning techniques. The study examines responses from 1,433 tech professionals to identify distinct patterns and clusters related to workplace mental health, support systems, and stigma perception.

### Key Objectives

- Identify distinct employee clusters based on mental health characteristics
- Analyze workplace factors affecting mental health outcomes
- Understand the interaction between organizational support, stigma, and professional treatment
- Provide data-driven insights for targeted mental health interventions

---

## 📊 Dataset Information

- **Source**: Mental Health in Tech Survey (Kaggle)
- **Size**: 1,433 respondents, 63 variables
- **Categories**:
  - Demographic information (age, gender, location)
  - Workplace characteristics (company size, remote work, industry)
  - Mental health benefits and resources
  - Personal mental health status and treatment history
  - Stigma and disclosure comfort levels

---

## 🔬 Methodology

### 1. Data Preprocessing

- Comprehensive missing value analysis and imputation
- Data type classification and handling
- Outlier detection using IQR method
- Feature standardization (mean=0, std=1)

### 2. Feature Engineering

- **Composite Scores**:
  - Mental Health Support Score (0-4)
  - Mental Health Stigma Score (0-3)
  - Work Interference Score (0-3)
- Interaction features (age-gender, treatment-disorder, etc.)
- Encoding strategies: Label encoding, One-hot encoding, Frequency encoding

### 3. Statistical Analysis

- Chi-Square tests for categorical associations
- ANOVA tests for numeric vs categorical comparisons
- Pearson and Spearman correlation analysis
- Cramér's V for effect size measurement

### 4. Feature Selection

- Mutual Information feature selection
- Chi-Square feature selection
- Recursive Feature Elimination (RFE)
- Composite importance scoring

### 5. Dimensionality Reduction

- **Principal Component Analysis (PCA)**: 95% variance retention
- **Multidimensional Scaling (MDS)**
- **Locally Linear Embedding (LLE)**
- **t-SNE** for visualization

### 6. Clustering Algorithms

- **K-Means Clustering** (k=2-10)
- **Hierarchical Clustering** (Ward linkage)
- **DBSCAN** (density-based)
- **Gaussian Mixture Models (GMM)**

### 7. Validation Metrics

- Silhouette coefficient
- Calinski-Harabasz index
- Davies-Bouldin index
- Gap statistic
- Dunn index

---

## 📈 Key Findings

### Demographic Insights

- **Age**: Mean 34.29 years, primarily 26-45 age group (88.2%)
- **Gender**: 69.1% Male, 23.0% Female, 3.4% Other
- **Location**: 54.4% United States, 22.3% United Kingdom

### Mental Health Insights

- **58.5%** have sought professional treatment
- **Two distinct clusters** identified:
  - **Cluster 1 (62.4%)**: Supportive workplace environments
  - **Cluster 2 (37.6%)**: Challenging environments with barriers

### Workplace Factors

- Company size concentration: 26-1000 employees
- Significant correlation between organizational support and treatment seeking
- Remote work patterns influence mental health disclosure comfort

---

## 🛠️ Technologies Used

### Core Libraries

- **Python 3.8+**
- **NumPy**: Numerical computing
- **Pandas**: Data manipulation and analysis
- **Matplotlib**: Data visualization
- **Seaborn**: Statistical visualization

### Machine Learning

- **scikit-learn**: ML algorithms and preprocessing
  - PCA, t-SNE, K-Means, DBSCAN, GMM
  - StandardScaler, LabelEncoder
  - Feature selection tools
  - Validation metrics

### Statistical Analysis

- **SciPy**: Statistical functions and tests
  - Chi-square, ANOVA, correlation tests
  - Winsorization for outlier handling

---

## 📁 Project Structure

```
mental-health-analysis/
│
├── mental health anaylsis.ipynb   # Main Jupyter notebook with complete analysis
├── mental-health.csv              # Dataset
├── README.md                      # Project documentation (this file)
├── requirements.txt               # Python dependencies
```

---

## 🚀 Getting Started

### Prerequisites

- Python 3.8 or higher
- Jupyter Notebook or JupyterLab
- pip package manager

### Installation

1. **Clone the repository**

```bash
git clone https://github.com/Justin10-nesto/mental-health-analysis.git
cd mental-health-analysis
```

1. **Create virtual environment (recommended)**

```bash
python -m venv venv

# On Windows
venv\Scripts\activate

# On macOS/Linux
source venv/bin/activate
```

1. **Install required packages**

```bash
pip install -r requirements.txt
```

1. **Launch Jupyter Notebook**

```bash
jupyter notebook
```

1. **Open the notebook**

- Navigate to `mental health anaylsis.ipynb`
- Run cells sequentially or use "Run All"

---

## 📓 Notebook Contents

### Part 1: Data Exploration

1. Initial data loading and exploration
2. Data types and missing values analysis
3. Missing data visualization
4. Column classification

### Part 2: Exploratory Data Analysis (EDA)

5. Age distribution analysis
2. Gender distribution analysis
3. Work environment analysis
4. Mental health benefits analysis
5. Mental health status analysis
6. Treatment seeking behavior
7. Stigma and disclosure analysis
8. Geographic distribution
9. Bivariate analysis
10. Key insights summary

### Part 3: Statistical Testing

15. Chi-square tests for categorical associations
2. ANOVA tests
3. Correlation significance tests

### Part 4: Feature Engineering

18. Missing value handling strategy
2. Composite score creation
3. Interaction feature engineering
4. Categorical variable cardinality analysis
5. Encoding (binary, label, one-hot, frequency)
6. Feature selection (MI, Chi2, RFE)

### Part 5: Preprocessing

24. Outlier detection and visualization
2. Outlier handling (winsorization)
3. Feature scaling (standardization)
4. Correlation analysis
5. Highly correlated feature removal

### Part 6: Dimensionality Reduction

29. PCA analysis
2. Comparison: PCA vs MDS vs LLE vs t-SNE

### Part 7: Clustering Analysis

31. K-Means clustering (optimal k selection)
2. Hierarchical clustering
3. DBSCAN clustering
4. Gaussian Mixture Models
5. Cluster validation and interpretation

---

## 📊 Results Interpretation

### Cluster Profiles

**Cluster 1: Supportive Environment (62.4%)**

- Higher mental health support scores
- More comfortable discussing mental health
- Better access to resources
- Lower perceived stigma

**Cluster 2: Challenging Environment (37.6%)**

- Limited organizational support
- Higher stigma perception
- Less comfortable with disclosure
- Fewer accessible resources

### Principal Components (PCA)

- **5 main components** explain 82.7% of variance
- Components represent:
  1. Organizational support factor
  2. Stigma and disclosure comfort
  3. Work interference and productivity
  4. Treatment and family history
  5. Demographic and workplace characteristics

---

## 💡 Recommendations

### For Organizations

1. **Enhance Mental Health Benefits**: Provide comprehensive, accessible mental health coverage
2. **Reduce Stigma**: Foster open communication about mental health without fear of career impact
3. **Training Programs**: Educate managers and colleagues on mental health awareness
4. **Flexible Work Arrangements**: Support work-life balance through remote work options
5. **Regular Assessment**: Conduct periodic mental health climate surveys

### For Policymakers

1. Mandate mental health coverage in tech industry employment packages
2. Establish industry-wide mental health standards
3. Support research on workplace mental health interventions

### For Individuals

1. Seek professional help without hesitation
2. Utilize available organizational resources
3. Participate in peer support networks
4. Advocate for better mental health policies

---

## 📚 Academic Significance

### Contributions

1. **Academic**: Replicable framework for unsupervised learning on psychological data
2. **Methodological**: Demonstrates unsupervised learning's exploratory capacity
3. **Organizational**: Actionable insights for tech companies
4. **Public Health**: Reduces economic and human burden of mental health disorders

### Research Questions Addressed

- What distinct employee clusters exist based on mental health characteristics?
- Which variables predict mental health outcomes?
- How do support systems, stigma, and treatment interact?
- What are key underlying components of mental health variance?
- How can organizations use these insights for targeted interventions?

---

## 🔍 Limitations

1. **Cross-sectional Design**: Cannot establish causality
2. **Self-reported Data**: Potential response bias
3. **Sample Demographics**: Predominantly male, English-speaking countries
4. **Missing Data**: 44/63 columns contain missing values
5. **Temporal Aspect**: Data represents single point in time

---

## 🔮 Future Work

1. **Longitudinal Study**: Track mental health changes over time
2. **Deep Learning**: Apply neural networks for pattern discovery
3. **Sentiment Analysis**: Analyze open-ended text responses
4. **Predictive Modeling**: Supervised learning for outcome prediction
5. **Cross-industry Comparison**: Compare tech vs non-tech sectors
6. **Intervention Studies**: Test effectiveness of recommended policies

---

## 👥 Contributors

- **Student Name**: Justini Lasway
- **Course**: Unsupervised Machine Learning
- **Institution**: UI International University
- **Semester**: III

---

## 📄 License

This project is for academic purposes. The dataset is publicly available on Kaggle under its respective license.

---

## 📧 Contact

For questions or collaboration opportunities:

- **Email**: <justini.lasway@iu-study.org>
- **GitHub**: [Justin10-nesto](https://github.com/Justin10-nesto)
- **LinkedIn**: [Justini Lasway](https://tz.linkedin.com/in/justini-lasway-b57173300)

---

## 🙏 Acknowledgments

- Kaggle for providing the Mental Health in Tech Survey dataset
- UI International University faculty for guidance
- The tech community for raising awareness about mental health
- World Health Organization for mental health research and statistics


## ⭐ Project Status

**Status**: ✅ Complete

**Last Updated**: February 2026

---

*This project demonstrates the application of unsupervised machine learning techniques to real-world mental health data, providing valuable insights for improving workplace mental health support systems in the technology industry.*
