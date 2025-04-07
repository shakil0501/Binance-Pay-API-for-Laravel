# Binance-Pay-API-for-Laravel

Binance Pay API for PHP and Laravel - This is a simple and quick package on how to initiate crypto payments using the Official Binance API. You can use this to initiate ecommerce payments or any other payments of your choose from your website.

Binance Pay API
To authenticate requests in the Binance Pay API, API keys are used. You can view and manage your API keys in the Binance Merchant Admin Portal.

Since API keys carry numerous privileges, it is essential to keep them secure. Avoid sharing your secret API keys in publicly accessible places like GitHub, client-side code, and similar locations.

It is mandatory to make all API requests over HTTPS. Calls made over plain HTTP will not succeed. Also, requests without authentication will fail.

Installation
You can install the package via composer:

composer require crypto-pay/binancepay
Get API Credentials#
Binance uses the Binance Pay API keys to authenticate API requests. You can view and manage your API keys in the Binance Merchant Admin Portal.

Go to: Developers → Settings → API Keys → Generate API Key

Read more...

Configurations
BINANCE_SERVICE_BASE_URL=https://bpay.binanceapi.com
BINANCE_SERVICE_RETURN_URL="/binancepay/returnUrl" # The URL to redirect to when the payment is successful.
BINANCE_SERVICE_CANCEL_URL="/binancepay/cancelURL" # The URL to redirect to when payment is failed.
BINANCE_SERVICE_WEBHOOK_URL="webhook-url"
BINANCE_MERCHANT_API_KEY=<api-key>
BINANCE_MERCHANT_SECRET_KEY=<secret-key>
