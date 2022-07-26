# Setting your Primary name

The Primary record is your _reverse record_ responsible for resolving your wallet address to your ENS name, effectively helping DApps and other services display your ENS name based on your wallet address_._

The easiest way to understand it is to consider that name resolution works in two directions:

### Forward resolution

* **Your ENS name ➞ Your wallet address,** or for a practical example:\
  **cthulu.eth ➞ 0x4b131a5b4c42cb703f360377beb262262821ca66**\
  ****_Determined by the ETH Address (forward) record set on your domain._

### Reverse resolution

* **Your wallet address ➞ Your ENS name,** or for a practical example: **0x4b131a5b4c42cb703f360377beb262262821ca66 ➞ cthulu.eth**\
  ****_Determined by the Primary (reverse) record set in your wallet._

In order to set an ENS name as Primary in a wallet, it's therefore a requirement that the ENS name first resolves to that wallet address.

In order to set your ENS name as Primary in your wallet:

1. Make sure the ETH-Address record points to the wallet address
2. Connect your wallet to the [ENS Manager App](https://app.ens.domains) and set the ENS name as Primary.
