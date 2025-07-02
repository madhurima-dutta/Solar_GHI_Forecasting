# Solar GHI Day-Ahead Forecasting Assessment

Expert Data Science Solution for predicting day-ahead Global Horizontal Irradiance (GHI) using historical environmental and irradiance features.

##  Quick Start

### Prerequisites
- Python 3.8+
- pip or conda

### Installation

1. **Clone the repository**
```bash
git clone <repository-url>
cd solar-ghi-forecasting
```

2. **Install Python dependencies**
```bash
pip install -r requirements.txt
```

3. **Run the assessment**
```bash
python scripts/solar_ghi_forecasting.py
```

### Using Docker

1. **Build and run with Docker**
```bash
docker-compose up --build
```

##  Features

- **Advanced Data Preprocessing**: Handles missing values, outliers, and feature engineering
- **Multiple ML Models**: Random Forest and XGBoost with hyperparameter optimization
- **Robust MAPE Calculation**: Handles zero values and prevents extreme outliers
- **Comprehensive Evaluation**: Monthly MAPE analysis and detailed performance metrics
- **Professional Visualizations**: Feature importance, prediction plots, and data exploration

##  Project Structure

```bash
solar-ghi-forecasting/
├── scripts/
│   ├── solar_ghi_forecasting.py    # Main forecasting script
│   └── run_assessment.py           # Quick runner script
├── outputs/                        # Generated results and plots
├── requirements.txt                # Python dependencies
├── package.json                    # Node.js metadata (for deployment)
├── Dockerfile                      # Docker configuration
├── docker-compose.yml              # Docker Compose setup
└── README.md                       # This file
```

##  Usage

### Basic Usage
```bash
python scripts/solar_ghi_forecasting.py
```

### Output Files
- `DataScientist.csv` - Main results with predictions and MAPE
- `monthly_mape.csv` - Monthly average MAPE values
- Various PNG plots for visualization

##  Model Performance

The solution implements:
- **Feature Engineering**: Time-based features, cyclical encoding, interaction terms
- **Data Quality**: Robust handling of missing values and outliers
- **Model Selection**: Cross-validation based selection between RF and XGBoost
- **Evaluation**: MAPE calculation optimized for solar irradiance characteristics

##  Technical Details

### Key Features
- Handles zero GHI values (nighttime) properly in MAPE calculation
- Creates cyclical time features for better temporal modeling
- Implements robust scaling and outlier treatment
- Provides comprehensive data exploration and visualization

### Dependencies
- pandas, numpy: Data manipulation
- scikit-learn: Machine learning models and preprocessing
- xgboost: Gradient boosting model
- matplotlib, seaborn: Visualization

##  Assessment Requirements

- Data preprocessing with timestamp parsing and feature engineering  
- Multiple model comparison (Random Forest, XGBoost)  
- MAPE calculation for each prediction  
- Monthly average MAPE computation  
- Output files in required format  
- Feature importance and prediction visualizations  

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Add tests if applicable
5. Submit a pull request

## License

This project is licensed under the MIT License - see the LICENSE file for details.
