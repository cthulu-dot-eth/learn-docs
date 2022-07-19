# On- & Off-chain voting

There are two types of voting systems used by ENS:

### Off-chain voting

Off-chain voting has the benefit of being gas free and is commonly used as a temperature check before elevating seemingly successful proposals to an on-chain vote, so that users don't have to spend gas voting on proposals that are likely to fail. ENS utilizes the [Snapshot decentralized voting system](https://snapshot.org/) for all off-chain votes.

### On-chain voting

On-chain voting registers the results onto the Ethereum blockchain and becomes permanent. After an off-chain vote has been conducted and it appears to be successful, it's elevated to an on-chain vote before it comes into effect.

On-chain voting incurs gas costs, as your vote is registered onto the Ethereum blockchain itself to make it immutable, which is why it's not the only system used.

ENS utilizes the [Tally decentralized voting system](https://www.tally.xyz/) for all on-chain votes.
