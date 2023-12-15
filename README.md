# DEXTswap (aggregator widget)

(This is the public documentation repo for the DEXTSwap aggregator widget)

The **DEXTswap Aggregator Widget** allows websites to embed the DEXTswap aggregator for any blockchain where this feature is supported as in [DEXTools.io](https://www.dextools.io) app.

![image](https://github.com/dextools-io/aggregator-widget/assets/4454927/400250f1-a8b3-4d43-91c6-ed288ec2fcc7)


## Quick Example

A simple IFrame integration example follows:

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

**Please be aware that USE OF THIS WIDGET IFRAME FROM **localhost** domain WON'T WORK, use a real domain instead.**


## Customization options

The widget is configured adjusting following parts and query parameters of this URL:

```text
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
| ZKSYNC     | zksync    |
| BASE       | base      |
