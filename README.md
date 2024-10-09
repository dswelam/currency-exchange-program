# Currency Converter Program
---
## Overview
This Python program allows users to convert one currency to another, check the exchange rate between two currencies, and list all available currencies. It fetches data from an online currency conversion API and uses that information to provide real-time exchange rates.

### Features:
- **List Available Currencies:** Displays a list of all supported currencies along with their currency codes and symbols.
- **Convert Between Currencies:** Converts an amount from one currency to another based on the latest exchange rate.
- **Get Exchange Rate:** Retrieves the current exchange rate between two specified currencies.
- **Interactive Command Interface:** The program allows users to input commands like `list`, `convert`, and `rate` to interact with it.

## Requirements
To use this program, you need to have the following Python libraries installed:

- `requests`: This library is used to make API requests to get currency information and exchange rates.
- `pprint`: This library is used for neatly printing out JSON and other data structures.

You can install the `requests` library using pip if you don’t have it installed:
```bash
pip install requests
```

## Setup

1. Clone or download the script.
2. Make sure to install the `requests` module if it's not already installed (see the requirements section).
3. You can use this program immediately by running it in a Python environment.

## API Usage
The program uses the **Free Currency Converter API** to get real-time data. The base URL for the API and your API key are hardcoded into the script.

- **API Base URL**: `https://free.currconv.com/`
- **API Key**: The provided API key is `648a294296570e6f457e`. You may replace this with your own if necessary.

## How to Use
When you run the program, you will be greeted with a set of options that allow you to:

- **List Currencies:** Type `list` to view all available currencies.
- **Convert Between Currencies:** Type `convert` to perform currency conversion between two currencies.
  - The program will prompt you to enter the base currency, the amount you wish to convert, and the currency you wish to convert into.
- **Get Exchange Rate:** Type `rate` to get the current exchange rate between two currencies.
  - The program will ask for the base currency and the target currency.
- **Quit the Program:** Type `q` to quit the program.

### Example Commands:
- **list**: Shows all available currencies.
- **convert**: Converts a specified amount from one currency to another.
  - Example: If you want to convert 100 USD to EUR, you will input `USD`, `100`, and `EUR`.
- **rate**: Gets the exchange rate between two currencies.
  - Example: To check the exchange rate between USD and EUR, input `USD` and `EUR`.

### Sample Output:
```bash
Welcome to the currency converter!
List - lists the different currencies
Convert - convert from one currency to another
Rate - get the exchange rate of two currencies

Enter a command (q to quit): list
AED - United Arab Emirates Dirham - د.إ
AFN - Afghan Afghani - ؋
ALL - Albanian Lek - L
...

Enter a command (q to quit): convert
Enter a base currency: USD
Enter an amount in USD: 100
Enter a currency to convert to: EUR
100.0 USD is equal to 92.57 EUR

Enter a command (q to quit): rate
Enter a base currency: USD
Enter a currency to convert to: EUR
USD -> EUR = 0.9257
```

## Notes
- Ensure that you have an internet connection, as the program requires API access to retrieve up-to-date exchange rates and currency information.
- You can customize the `API_KEY` variable if you have a different API key for the currency conversion service.

## License
This program is free to use and distribute. You may modify it as needed. Be sure to comply with the terms of service of the API you are using.

---

Enjoy using the Currency Converter program!
