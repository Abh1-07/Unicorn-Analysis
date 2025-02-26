# Unicorn Startup Funding Analysis Dashboard

This repository contains a Power BI dashboard analyzing unicorn startup funding data up to March 2022.

## Dataset

The dataset is sourced from [Kaggle](https://www.kaggle.com/datasets/ramjasmaurya/unicorn-startups/data) and includes the following columns:

- Company
- Valuation ($B)
- Date Joined
- Country
- City
- Industry
- Investors
- Founded Year
- Fundings

## Data Preparation

The following transformations were applied to the dataset:

- **Fundings Column**: Standardized monetary values to integers representing millions.
- **Top 4 Investors**: Extracted the first four investors for each company.
- **Years to Unicorn Valuation**: Calculated the duration from the company's founding to achieving unicorn status.
- **Country to Continent Mapping**: Added a continent column based on each company's country.

## Power BI Model

The Power BI model consists of three tables:

- **Unicorns**: Main table with company information.
- **Fundings**: Contains 'Company' and 'Fundings' columns.
- **Investors**: Contains 'Company' and 'Top 4 Investors' columns.

Relationships were established between these tables using the 'Company' column as the key.

## Visualizations

The dashboard includes:

- Total valuation of all unicorns.
- Industry distribution of unicorns.
- Funding trends over time.
- Top investors in unicorn startups.
- Geographical distribution of unicorns by continent and country.

## Usage

To view and interact with the dashboard:

1. Clone this repository.
2. Open the `.pbix` file using [Power BI Desktop](https://powerbi.microsoft.com/desktop/).
