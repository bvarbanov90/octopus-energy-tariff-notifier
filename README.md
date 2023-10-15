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
