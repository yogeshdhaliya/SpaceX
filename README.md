# SpaceX Falcon 9 First Stage Landing Prediction

[![Python](https://img.shields.io/badge/python-v3.7+-blue.svg)](https://www.python.org/downloads/)
[![Jupyter](https://img.shields.io/badge/Made%20with-Jupyter-orange?logo=Jupyter)](https://jupyter.org/try)
[![IBM](https://img.shields.io/badge/IBM-Data%20Science%20Capstone-blue)](https://www.coursera.org/learn/applied-data-science-capstone)

## 📊 Project Overview

This repository contains the **IBM Data Science Capstone Project** focusing on predicting the success of SpaceX Falcon 9 first stage landings. As part of the IBM Data Science Professional Certificate program, this project demonstrates the complete data science methodology applied to real-world aerospace data.

### 🚀 Business Problem

SpaceX advertises Falcon 9 rocket launches at $62 million per launch, significantly lower than competitors who charge upwards of $165 million. This cost advantage stems from SpaceX's ability to reuse the first stage of the rocket. By accurately predicting first stage landing success, competing companies can make informed bidding decisions against SpaceX for rocket launch contracts.

### 🎯 Objective

Apply data science and machine learning techniques to predict whether SpaceX Falcon 9 first stage will land successfully, enabling competitive cost analysis for rocket launches.

## 📁 Repository Structure

```
├── 📁 Lab-1-Data-Collection-API/           # Data collection using SpaceX REST API
├── 📁 Lab-2-Data-Collection-WebScraping/   # Web scraping from Wikipedia
├── 📁 Lab-3-Data-Wrangling/               # Data cleaning and preprocessing  
├── 📁 Lab-4-EDA-SQL/                      # Exploratory analysis with SQL
├── 📁 Lab-5-EDA-Visualization/            # Data visualization and insights
├── 📁 Lab-6-Interactive-Visual-Analytics/ # Folium maps and Plotly dashboards
├── 📁 Lab-7-Machine-Learning-Prediction/  # ML models and hyperparameter tuning
├── 📁 Lab-8-Final-Report/                 # Executive summary and presentation
├── 📁 data/                               # Raw and processed datasets
├── 📁 images/                             # Visualizations and charts
├── 📄 README.md                           # Project documentation
└── 📄 requirements.txt                    # Python dependencies
```

## 🔬 Methodology

The project follows the **CRISP-DM** (Cross-Industry Standard Process for Data Mining) methodology:

### 1. **Data Collection** 
- **SpaceX REST API**: Launch records, rocket specifications, mission parameters
- **Web Scraping**: Wikipedia pages for comprehensive launch history
- **Data Sources**: 90+ Falcon 9 launches from 2010-2020

### 2. **Data Wrangling**
- Missing value treatment and data type conversions
- Feature engineering and categorical encoding
- Creation of binary target variable (landing success/failure)

### 3. **Exploratory Data Analysis**
- **SQL Analysis**: Launch trends, success rates, payload correlations
- **Statistical Analysis**: Success rates by launch site, orbit type, and payload mass
- **Visual Analytics**: Interactive dashboards and geospatial analysis

### 4. **Interactive Visualizations**
- **Folium Maps**: Launch site proximity analysis and geographical insights
- **Plotly Dash**: Interactive dashboard for launch record analysis
- **Plotly**: Dynamic scatter plots and success rate visualizations

### 5. **Machine Learning**
- **Algorithms Tested**: 
  - Logistic Regression
  - Support Vector Machines (SVM)
  - Decision Tree Classifier  
  - K-Nearest Neighbors (KNN)
- **Model Optimization**: GridSearchCV for hyperparameter tuning
- **Evaluation Metrics**: Accuracy, Precision, Recall, F1-Score

## 🛠️ Technologies Used

| Category | Technologies |
|----------|-------------|
| **Programming** | Python 3.7+ |
| **Data Manipulation** | Pandas, NumPy |
| **Data Visualization** | Matplotlib, Seaborn, Plotly |
| **Machine Learning** | Scikit-learn |
| **Web Scraping** | BeautifulSoup, Requests |
| **Interactive Maps** | Folium |
| **Dashboard** | Plotly Dash |
| **Database** | SQLite |
| **Development** | Jupyter Notebook |

## 📋 Prerequisites

- Python 3.7 or higher
- Jupyter Notebook or JupyterLab
- Internet connection (for API calls and web scraping)

## ⚙️ Installation & Setup

1. **Clone the repository**
```bash
git clone https://github.com/yogeshdhaliya/SpaceX.git
cd SpaceX
```

2. **Create virtual environment**
```bash
python -m venv spacex-env
source spacex-env/bin/activate  # On Windows: spacex-env\Scripts\activate
```

3. **Install dependencies**
```bash
pip install -r requirements.txt
```

4. **Launch Jupyter Notebook**
```bash
jupyter notebook
```

## 🚀 Usage

### Running Individual Labs

Navigate through the labs sequentially for the complete data science workflow:

1. **Lab 1**: Start with `Lab-1-Data-Collection-API.ipynb` to collect data from SpaceX API
2. **Lab 2**: Run `Lab-2-Data-Collection-WebScraping.ipynb` for web scraping  
3. **Lab 3**: Execute `Lab-3-Data-Wrangling.ipynb` for data preprocessing
4. **Lab 4**: Analyze with `Lab-4-EDA-SQL.ipynb` using SQL queries
5. **Lab 5**: Visualize insights in `Lab-5-EDA-Visualization.ipynb`
6. **Lab 6**: Create interactive analytics with `Lab-6-Interactive-Visual-Analytics.ipynb`
7. **Lab 7**: Build ML models in `Lab-7-Machine-Learning-Prediction.ipynb`
8. **Lab 8**: Review final report and presentation materials

### Running the Dashboard

```bash
cd Lab-6-Interactive-Visual-Analytics
python spacex_dash_app.py
```
Navigate to `http://127.0.0.1:8050/` to view the interactive dashboard.

## 📊 Key Findings

### 🎯 Model Performance
- **Best Performing Algorithm**: Decision Tree Classifier
- **Accuracy**: 87.5%
- **Key Success Factors**: 
  - Launch site location
  - Payload mass (optimal range: 2,000-5,500 kg)
  - Orbit type (GTO and LEO show higher success rates)
  - Flight number (success rate improves with experience)

### 📈 Business Insights
- **Success Rate Trend**: Significant improvement from 40% (2013) to 90%+ (2020)
- **Launch Site Analysis**: KSC LC-39A shows highest success rate (76.9%)
- **Payload Impact**: Heavy payloads (>6,000 kg) show reduced success probability
- **Cost Implications**: Successful landings save $100+ million per launch

## 🔍 Project Highlights

- **Real-world Data**: Utilized actual SpaceX launch data and operational parameters
- **End-to-End Pipeline**: Complete data science workflow from collection to deployment  
- **Interactive Components**: Dynamic dashboards and geospatial visualizations
- **Business Focus**: Practical application for competitive analysis in aerospace industry
- **Reproducible Research**: Well-documented notebooks with clear methodology

## 🏆 Skills Demonstrated

- **Data Engineering**: API integration, web scraping, data wrangling
- **Statistical Analysis**: Hypothesis testing, correlation analysis, trend identification  
- **Machine Learning**: Classification algorithms, hyperparameter tuning, model evaluation
- **Data Visualization**: Static plots, interactive dashboards, geospatial mapping
- **Business Intelligence**: Stakeholder reporting, actionable insights, cost-benefit analysis

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/improvement`)
3. Commit your changes (`git commit -am 'Add new feature'`)
4. Push to the branch (`git push origin feature/improvement`)  
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **IBM Data Science Professional Certificate** program
- **SpaceX** for providing public API access
- **Coursera** for the comprehensive learning platform
- **Wikipedia** community for maintaining detailed launch records

## 📞 Contact

- **GitHub**: [@yogeshdhaliya](https://github.com/yogeshdhaliya)
- **LinkedIn**: [Connect with me](https://linkedin.com/in/yogeshdhaliya)
- **Email**: [Your Email]

---

⭐ **Star this repository if you found it helpful!** ⭐

---

*This project demonstrates practical application of data science methodologies to real-world aerospace challenges, showcasing the complete pipeline from data collection to predictive modeling and business insights.*