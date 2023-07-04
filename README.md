# DEXTswap aggregator widget

(This is the public documentation repo of the DEXTswap aggregator widget)

The **DEXTswap Aggregator Widget** allows websites to embed DEXTswap aggregator for any blockchain where such feature is supported. Same as in [DEXTools.io](https://www.dextools.io) app.

# TODO: Add widget screenshot


## Get your DEXTswap iframe widget code

# TODO: describe steps to get the widget url, still not available


## Quick Example

A iframe based integration example follows:

```html
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>DEXTswap Aggregator Widget Template</title>
</head>

<body>

   <iframe id="dextswap-aggregator-widget"
    title="DEXTswap Aggregator"
    width="400"
    height="420" src="https://www.dextools.io/widget-aggregator/en/swap/eth/0xfb7b4564402e5500db5bb6d63ae671302777c75a"></iframe>

</body>
</html>

```

## Common issues and testing

You can test if the IFrame integration works properly with the https://iframetester.com/ tool.

In case the widget does not display prices and/or balances in your website, please check your CSP policy for IFrame content https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-Frame-Options


## Customization options

The widget is configured adjusting following parts and query parameters of this URL:

```
https://www.dextools.io/widget-aggregator/en/swap/<chainId>/<tokenAddress>?theme=<theme>
```

| Parameter    | Values                                                                                                                                                                                                                            |
|--------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| chainId      | blockchain ID (see [list below](#supported-blockchains))                                                                                                                                                                          |
| tokenAddress | address of the token to be used as `token-in` (the token to buy).<br/>The `token-out` is automatically set according to the chain's reference token, i.e. `ETH` for Ethereum, `BNB` for BNB Chain, `Matic` for Polygon and so on. |
| theme        | `dark` or `light`                                                                                                                                                                                                                 |


## Supported blockchains

This is the current list of blockchains supported:

| Blockchain | ID        |
|------------|-----------|
| ETHEREUM   | eth       |
| BNB        | bnb       |
| POLYGON    | polygon   |
| FANTOM     | fantom    |
| CRONOS     | cronos    |
| ARBITRUM   | arbitrum  |
| AURORA     | aurora    |
| AVALANCHE  | avalanche |
| OPTIMISM   | optimism  |
