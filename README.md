# NYC Airbnb Market Analysis — EDA

An exploratory data analysis of ~102,000 NYC Airbnb listings, looking at pricing, room types, borough trends, and review activity over time.

## Project Goal

Airbnb listing data is a rich source for understanding pricing patterns, location trends, and host behavior. 
This project cleans a raw NYC Airbnb listings dataset and explores:

- How are listing prices distributed, and does room type actually affect price?
- Which boroughs have the most listings, and how does that relate to price?
- What do review patterns over time reveal — including possible data quality issues?
- Does host identity verification relate to price or reviews?

## Dataset

- **Size:** ~102,599 rows, 26 columns
- **Key fields:** price, room type, borough/neighbourhood, minimum nights, number of reviews, last review date, availability

## Tools Used

- Python
- Pandas, NumPy — data cleaning and manipulation
- Matplotlib, Seaborn — visualization

## Key Findings

- Prices are broadly spread across $50–$1,200 with no single dominant "typical" price.
- *Entire home/apt* is the most listed room type, followed closely by *private room*; shared and hotel rooms are rare.
- Manhattan and Brooklyn dominate listing volume; Queens, the Bronx, and Staten Island have far fewer listings.
- Median prices are surprisingly similar (~$620–$655) across all room types a signal worth investigating further, as it doesn't match typical Airbnb pricing patterns.
- Review activity over time shows two unusual spikes (~2019 and ~2022), likely from missing/defaulted review dates rather than real booking surges.

## Next Steps

- Neighbourhood-level (not just borough-level) price mapping
- A simple price prediction model using room type, borough, and availability as features
- Geographic visualization using latitude/longitude
