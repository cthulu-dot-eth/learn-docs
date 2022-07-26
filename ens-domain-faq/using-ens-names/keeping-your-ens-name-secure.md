# Keeping your ENS name secure

It is important to store your ENS name securely. If the ENS name is lost or stolen, it would be like losing your identity in Web3. You should always practice best security, like never giving out your seed phrases or private keys to anyone for any reason. Some users of ENS prefer to store their name in a cold wallet. This would mean that the Registrant record for the ENS name is set to the cold wallet. This wallet would be the **owner** of the ENS name. Whichever wallet is the Registrant, has access to transfer the name ownership to another wallet. ENS names are [ERC721](https://ethereum.org/en/developers/docs/standards/tokens/erc-721/) compliant NFTs on the Ethereum blockchain.

In some scenarios, ENS name owners choose a combination of both a cold wallet and hot wallet. So for instance, the ownership(Registrant) of the name would be set to a cold wallet like Ledger or Trezor while the Controller would be set to a hot wallet like MetaMask. This way the ownership of the name is safely held in a cold wallet, but a hot wallet can be used to update records like ETH payment addresses or other records of the ENS name besides the Registrant.

The ETH Address record, which is the _forward_ resolution of the ENS name, could be set to a wallet address that is different from the Registrant and Controller records.

### Further reading

{% content-ref url="../names-and-records/how-does-name-resolution-work.md" %}
[how-does-name-resolution-work.md](../names-and-records/how-does-name-resolution-work.md)
{% endcontent-ref %}

{% content-ref url="../names-and-records/what-is-a-primary-name.md" %}
[what-is-a-primary-name.md](../names-and-records/what-is-a-primary-name.md)
{% endcontent-ref %}
