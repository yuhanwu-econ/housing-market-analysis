# Cost-Benefit Analysis: Renting vs. Buying a Home in U.S. Cities

## Overview
- Evaluates the long-term financial trade-offs between renting and buying a home across the 50 most populous U.S. cities.
- Uses net present value (NPV) to compare both options over 15-year and 30-year horizons.
- Key Finding: Buying a home strictly dominates renting in all analyzed cities for both timeframes.

## Data Sources
- **Home prices**: Zillow Home Value Index (ZHVI), 35th–65th percentile range, Jan 2000–Mar 2025
- **Rental prices**: Zillow Observed Rent Index (ZORI), 35th–65th percentile range, Jan 2015–Mar 2025
- **Property tax rates**: Tax Foundation (2023 median state rates)

Files included:
- `Metro_zhvi_uc_sfrcondo_tier_0.33_0.67_sm_sa_month.csv`
- `Metro_zori_uc_sfrcondomfr_sm_month.csv`

## Methodology
- **Time Horizons**: 15 years and 30 years
- **Assumptions**:
  - Buyers:
    - Down payment: 20%
    - Mortgage rates: 6.83% (30-year), 6.03% (15-year) from FRED as of April 2025
    - Home insurance & maintenance: 1.5% of home value annually
    - Transaction costs: 3% purchase, 8% sale
  - Renters:
    - Rental insurance: 1% of annual rent
    - Rental inflation: city-specific Compound Annual Growth Rate (CAGR) (2015–2025)

- **NPV Calculations**:
  - Buying: Includes upfront costs, annual costs (mortgage, insurance, property taxes), and proceeds from the eventual sale (discounted).
  - Renting: Includes total rent payments, inflation-adjusted, plus rental insurance, discounted at 5%.

## Results
- Buying is financially more favorable than renting in all 50 cities, even under conservative assumptions.
- Both renting and buying have negative NPVs — neither is strictly profitable over time.
- Buying minimizes financial losses compared to renting.

## Repository Structure
- `Cost Benefit Analysis.ipynb` – Full Jupyter Notebook with analysis
- `Cost Benefit Analysis.pdf` – Final written report
- `README.md` – Project documentation
- `Data` - CSV files listed above

## Limitations & Considerations
- Financial perspective only — does not include:
  - Liquidity constraints
  - Lifestyle flexibility
  - Transaction complexity
- Assumes fixed mortgage rates and median property tax rates.


