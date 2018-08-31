# bitfinex historical data
In this repository you will find 1 minute candles (open/close/highest/lowest/volume) from bitfinex for the pairs:

*  **BTC/USD**
*  **ETH/USD**
*  **EOS/USD**
*  **LTC/USD**
*  **XRP/USD**
*  **IOT/USD**
*  **NEO/USD**

The format is [timestamp (UTC/milliseconds)],[open price],[close price],[highest price],[lowest price],[volume].

The Bitfinex API allows to receive up to 120 records per request. Because of this, I use a period of 2 hours (120 1m candles) per request. You can find the response from the Bitfinex server in the "raw" folder in each currency pairs. Because there is a rate limit of approx. 10 request per minute, it takes hours and thousands of requests to fetch the data of a whole year. The use of this project is to offer you a quick and easy way, to access the historical data, and relieve the bitfinex server from that much of requests.

The merged.json and merged.csv are generated by pure text-processing. The values are not parsed in any way. That means, there is no rounding error or loss of precision compared to the raw data.

The data are provided as-is without any warranty. Use it at your own risk.