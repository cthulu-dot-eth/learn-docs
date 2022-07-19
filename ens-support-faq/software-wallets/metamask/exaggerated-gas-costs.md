# Exaggerated gas costs

Metamask has a [known bug](https://github.com/MetaMask/metamask-extension/issues/13135) where users are shown an incredibly high gas fee estimate if there isn't enough ETH in the wallet to cover the _actual_ transaction costs.

![](<../../../.gitbook/assets/metamask\_exaggerated\_gas (1).png>)

This can be solved by transferring more ETH into the wallet to cover the _actual_ transaction cost which should be a lot less than what Metamask shows when it's encountering this bug.

