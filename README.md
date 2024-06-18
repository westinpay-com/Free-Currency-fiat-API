# WestinPay Currency Rates API

WestinPay's Free Currency Fiat API provides real-time exchange rates and currency conversion for over 152 currencies. It's ideal for financial apps, e-commerce platforms, and travel services.

## Endpoint

The WestinPay Currency Rates Endpoint delivers real-time exchange rates.

### Authentication

Once you have created an account on [WestinPay](https://westinpay.com/merchant/register), your account will be assigned a unique 32-character API key. Think of this like a secure password; keep it safe and do not share it with others.

### Parameters

- **base**: The base currency for conversion. Default is USD.
- **output**: Response format, either JSON or XML. Default is JSON.
- **api_key**: Your unique API key. Replace YOUR-API-KEY with your actual API key.

### Code Example

To fetch the latest rates using cURL and authenticate with your API key, use the following command:

```sh
curl --location --request GET 'https://westinpay.com/currency/fiat_api?api_key=YOUR-API-KEY&base=USD&output=JSON'


<details>
<summary>Response Example</summary>

```json
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
</details>
```









