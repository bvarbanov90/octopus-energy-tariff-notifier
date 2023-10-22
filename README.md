# Octopus Tariff Price Notification

## Overview

This project fetches and compares energy tariff prices from the Octopus API. It sends notifications regarding daily energy prices.

## Setup

1. Clone the repository.
2. Navigate to `OctopusTarrifPriceNotification` folder.
3. Update `config.json` with your credentials and settings.

## How to Run

Execute the Jupyter Notebook `OctopusTarrifPriceNotification.ipynb`.

## Dependencies

- `requests`
- `json`
- `smtplib`
- `datetime`

## Example Output

### Electricity
[Octopus] Daily Energy Prices Notification  
Tarrif electricity-tariffs/E-1R-SILVER-FLEX-22-11-25-A price comparison for 2023-10-15:  
Price today: 16.87 p/kWh  
Price tomorrow: 23.94 p/kWh  
Average price yesterday(2023-10-14): 17.52 p/kWh, Absolute Change: -0.65 p/kWh, % Change: -3.70%  
...  

### Gas

[Octopus] Daily Energy Prices Notification  
Tarrif gas-tariffs/G-1R-SILVER-FLEX-22-11-25-A price comparison for 2023-10-15:  
Price today: 6.35 p/kWh  
Price tomorrow: 6.42 p/kWh  
Average price yesterday(2023-10-14): 6.37 p/kWh, Absolute Change: -0.02 p/kWh, % Change: -0.33%  
...  

# Octopus Tariff Analysis and Forecasting

## Overview

This project is focused on analyzing energy tariffs from the Octopus Energy API and forecasting future prices using the Prophet library. The analysis is performed via a Jupyter Notebook and the results are visualized using Plotly.

**Copyright**: 2023 Borislav Rumenov Varbanov  
**License**: Apache License, Version 2.0

## Requirements

- Python 3.11
- Jupyter Notebook
- Plotly
- Pandas
- Prophet
- Scipy
- Requests

## Configuration

The `config.json` file is required for setting the API key, product code, tariff codes, and other parameters.

## Features

- Fetches tariff data from Octopus Energy API.
- Saves the fetched data to a CSV file.
- Conducts time-series analysis to find monthly average prices.
- Identifies anomalies in the energy prices.
- Uses Prophet to forecast future energy prices for the next three months.
- Provides interactive visualizations using Plotly.

## Usage

1. Clone the repository.
2. Navigate to the project directory and install the required packages.
3. Update the `config.json` file with the necessary configurations. API_KEY as a mandatory minimum!
4. Open `OctopusTariffAnalysisAndProphet.ipynb` in Jupyter Notebook.
5. Run all cells to perform the analysis and generate plots.

## Example of output figure plots in HTML
### Monthly energy prices
![image](https://github.com/bvarbanov90/octopus-energy-tariff-notifier/assets/5960215/5c208192-09df-4097-9385-6c5bed082177)
![image](https://github.com/bvarbanov90/octopus-energy-tariff-notifier/assets/5960215/f82ade54-8704-4dc8-a0cc-4942cd858147)

### Energy Prices with Anomalies
![image](https://github.com/bvarbanov90/octopus-energy-tariff-notifier/assets/5960215/8f15759f-1213-45b8-a8e0-37583d75c980)

### Electricity Tariff Price Forecast for Next 3 Months
![image](https://github.com/bvarbanov90/octopus-energy-tariff-notifier/assets/5960215/111ce6bb-3484-4fc3-99d7-7227f2db41ae)

### Gas Tariff Price Forecast for Next 3 Months
![image](https://github.com/bvarbanov90/octopus-energy-tariff-notifier/assets/5960215/0a3fac8c-312c-4476-b5c3-efa455a84b51)

