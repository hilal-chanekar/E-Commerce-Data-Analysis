# E-Commerce Data Analysis Project

## Overview
This project performs comprehensive data cleaning and analysis on the Brazilian E-Commerce dataset from Kaggle. The dataset contains transaction data from the Olist marketplace, including orders, customers, products, reviews, payments, sellers, and geolocation information.

## Project Structure
```
├── cleaning.ipynb          # Main notebook for data loading and cleaning
├── README.md              # Project documentation
└── venv/                  # Python virtual environment
```

## Dataset Information
The project works with the following datasets from the Olist Brazilian E-Commerce dataset:
- **olist_orders_dataset**: Order information and order status
- **olist_customers_dataset**: Customer data and demographics
- **olist_products_dataset**: Product catalog and details
- **olist_order_reviews_dataset**: Customer reviews and ratings
- **olist_order_payments_dataset**: Payment methods and amounts
- **olist_sellers_dataset**: Seller information
- **olist_geolocation_dataset**: Geographic location data
- **product_category_name_translation**: Product category translations

## Notebook Contents
### `cleaning.ipynb`
The main notebook contains the following sections:
1. **Data Import**: Downloads and loads the Brazilian E-Commerce dataset using Kaggle API
2. **Data Exploration**: Lists all datasets and displays column information
3. **Duplicate Analysis**: Identifies and analyzes duplicate records in key identifier columns:
   - Checks for duplicates in primary key columns for each dataset
   - Calculates duplicate percentages
   - Displays top duplicate values
   - Generates a summary table of findings

## Requirements
- Python 3.8+
- pandas
- kagglehub

## Installation & Setup

### 1. Create Virtual Environment
```bash
python -m venv venv
source venv/bin/activate
```

### 2. Install Dependencies
```bash
pip install pandas kagglehub jupyter
```

### 3. Kaggle API Setup
- Download your Kaggle API key from https://www.kaggle.com/settings/account
- Place it in `~/.kaggle/kaggle.json`
- Ensure proper permissions: `chmod 600 ~/.kaggle/kaggle.json`

### 4. Run the Notebook
```bash
jupyter notebook cleaning.ipynb
```

## Key Analysis Features
- **Automatic Type Inference**: DataFrames are loaded with optimized type detection
- **Duplicate Detection**: Comprehensive duplicate analysis across all datasets
- **Key Metrics**: Generates summary statistics including:
  - Total rows and unique values
  - Duplicate count and percentage
  - Top duplicate entries

## Usage
Execute the notebook cells sequentially:
1. Import libraries
2. Download dataset from Kaggle
3. Load all CSV files into a dictionary of DataFrames
4. Run duplicate analysis to identify data quality issues

## Data Quality Insights
The duplicate analysis helps identify:
- Data integrity issues in key identifiers
- Potential data entry errors
- Datasets requiring additional cleaning

## Future Enhancements
- Data type optimization and conversion
- Missing value imputation
- Outlier detection and handling
- Feature engineering for analysis
- Statistical summary generation

## Notes
- Dataset is downloaded dynamically from Kaggle on first run
- All data is stored in DataFrames for in-memory analysis
- Results are printed to console with formatted output

## License
Data sourced from Kaggle's Brazilian E-Commerce dataset by Olist

## Author
Data Analysis Team
