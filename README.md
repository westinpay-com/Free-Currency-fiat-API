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
