# WestinPay-Currency-Rates-API-cURL-Example
WestinPay's Free Currency Fiat API delivers real-time exchange rates and currency conversion. Ideal for financial apps, e-commerce platforms, and travel services.
# WestinPay Currency Rates Endpoint

## Overview

The WestinPay Currency Rates Endpoint provides real-time exchange rates for over 152 currencies.

### Parameters

- **base**: The base currency for the conversion. Default: USD.
- **output**: Response output in either JSON or XML. Default: JSON.

### Code Example

Fetch the latest rates using the curl command:

```sh
curl --location --request GET 'https://westinpay.com/currency/fiat_api?api_key=YOUR-API-KEY&base=USD&output=JSON'

Response
The response will be in JSON format and will include the following structure:

json

{
  "valid": true,
  "updated": 1526293289,
  "base": "USD",
  "rates": {
    "AED": 5.2204725081026,
    "AFN": 99.505376130096,
    "ALL": 148.13498464775,
    "AMD": 683.01869278444,
    "ANG": 2.5307798373799,
    ...
  }
}
