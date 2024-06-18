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



  <section id="response" class="section">
                  <h1>Response</h1>
                <p>By default, our API response is in JSON.</p>
                <p>You can select to output in XML on any of our API by passing the output parameter to equal xml.</p>
                <p>Correctly formatted requests return a 200 HTTP response code.</p>
                <p>Incorrect or incomplete requests return a 400 HTTP response code.</p>
                <p>We also return an error code in the body of our response to help you identify the issue with the request. See the full list of these below.</p>
                <div class="terminal">
                    <pre>{
  "valid": true,
  "updated": 1526293289,
  "base": "GBP",
  "rates": {
      "AED": 5.2204725081026,
      "AFN": 99.505376130096,
      "ALL": 148.13498464775,
      "AMD": 683.01869278444,
      "ANG": 2.5307798373799,
      // other rates...
  }
}</pre>
                </div>
            </section>

