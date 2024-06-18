# WestinPay Currency Rates API

WestinPay's Free Currency Fiat API provides real-time exchange rates and currency conversion for over 152 currencies. It's ideal for financial apps, e-commerce platforms, and travel services.

## Endpoint

The WestinPay Currency Rates Endpoint delivers real-time exchange rates.

### Authentication

Once you have created an account on [WestinPay](https://westinpay.com/merchant/register), your account will be assigned a unique 32-character API key. Think of this like a secure password; keep it safe and do not share it with others.

### Parameters

- **base**: The base currency for conversion. Default is USD.
- **output**: Response format, either JSON or XML. Default is JSON.
- **api_key**: Your unique API key. Replace YOUR_API_KEY with your actual API key.

### Code Example

To fetch the latest rates using cURL and authenticate with your API key, use the following command:

```sh
curl --location --request GET 'https://westinpay.com/currency/fiat_api?api_key=YOUR-API-KEY&base=USD&output=JSON'
