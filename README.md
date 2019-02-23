The Niobio Cash is the Brazilian national cryptocurrency, just like Bitcoin but more anonymous and privacy centric with opaque and more analysis resistant blockchain. It is people's electronic cash, not connected to government or officials.

# Auxiliary Files for Niobio Cash Wallets
Files on this repository are read by Niobio Cash wallets to update internal lists dinamically.
## Wallet Nodes File
The file *wallet-nodes.txt* contain the list of active wallet nodes that can be used by desktop wallets to interact with the blockchain without downloading the blocks.

More information about Wallet Nodes can be found at https://github.com/niobio-cash/ncip/blob/master/ncip-0004.mediawiki

If you want to run a wallet node you can make a pull request to this repository, including your nodes's url as a new line **at bottom**.

Alternatively, you can open an issue asking us to include it.

To download the daemon that runs the node's service, access https://github.com/niobio-cash/niobio-node-daemon/releases and get the last release.

You must use the command line options that inform to the node your wallet address and the fee you want to charge users by each sending transfer they do using your wallet node.

This example is for Linux and MacOS platforms.

/<path>/niobiod --enable-blockchain-indexes --restricted-rpc --rpc-bind-ip 0.0.0.0 --fee-address <fee Address> --fee <fee>

Replace <fee Address> and <fee> with you wallet address and the percentual fee (such as 0.15).
