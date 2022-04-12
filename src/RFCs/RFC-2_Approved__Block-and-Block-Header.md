# RFC 2 WIP: Block and Block Header

This RFC describes the block structure and the block header to be used in the doc-chain project.

## The Block Header

The structure of the block header is almost the same as Bitcoin's.
The block header is an efficient way of storing the block on the blockchain.
It consists of three components:

- **Previous Hash**: The hash of the previous block.
- **Nonce**: The proof-of-work generated in the mining process. Useful in verifying the integrity of the blockchain.
- **Merkle Root**: The merkle root of all the documents in the block. As described in [The Bitcoin White Paper](https://bitcoin.org/en/bitcoin-paper)

## Block

All the blocks collectively store all the documents in the blockchain.
Specifically the document checksums and document header.
It consists of:

- **The block header**: As described above. The only piece which is stored on the blockchain.
- **All the document headers**: All the document headers. The real need of authenticity is for these.

The document headers will be checked before the block is added.
