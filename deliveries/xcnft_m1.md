# Milestone Delivery :mailbox:

**The delivery is according to the official [milestone delivery guidelines](https://github.com/w3f/Grants-Program/blob/master/docs/Support%20Docs/milestone-deliverables-guidelines.md).**  

* **Application Document:** [xcNFT.md](https://github.com/w3f/Grants-Program/blob/master/applications/xcNFT.md)
* **Milestone Number:** 1

**Context** 

Milestone delivered the first pallet-agnostic cross-chain NFT pallet on Polkadot called xcNFT. 

**Deliverables**
| Number | Deliverable | Link | Notes |
| ------------- | ------------- | ------------- |------------- |
| 0a. | License |[MIT xcNFT](https://github.com/paraspell-research/xcnft-pallet/blob/main/LICENSE), [MIT DOCS](https://github.com/paraspell-research/xcnft-docs/blob/main/LICENSE)| MIT| 
| 0b.  | Documentation |[Main xcNFT readme](https://github.com/paraspell-research/xcnft-pallet/blob/main/README.md), [xcNFT pallet_nfts readme](https://github.com/paraspell-research/xcnft-pallet/tree/main/xcnft-pallet_nfts), [xcNFT pallet_uniques readme](https://github.com/paraspell-research/xcnft-pallet/blob/main/xcnft-pallet_uniques/README.md), [official documentation](https://paraspell-research.github.io/xcnft-docs/)| Readmes for all major parts of repository + inline documentation in each version of pallet + official documentation | 
| 0c.  | Testing guide | [Testing guide in readme](https://github.com/paraspell-research/xcnft-pallet/blob/main/README.md#testing-pallet-functionality-), [Testing guide in docs](https://paraspell-research.github.io/xcnft-docs/implementation-guide/introduction.html#testing-pallet-functionality-%F0%9F%94%8E), [Unit tests commit](https://github.com/paraspell-research/xcnft-pallet/commit/c6682ecdf2fe9fdc51a678b028d77a0a4e33efa6) |  Testing guide mentioned in readme and official docs & core unit tests | 
| 0d.  | Docker | [Docker guide](https://github.com/paraspell-research/xcnft-pallet/blob/main/README.md#dockerized-local-testnet-build), [Dockerfile](https://github.com/paraspell-research/xcnft-pallet/blob/main/Dockerfile)| Docker file provided to test the functionality of the solution | 
| 1 | xcNFT Bump dependencies |[Commit adding latest frame version compliant xcNFT](https://github.com/paraspell-research/xcnft-pallet/commit/99a1202fd258c5bc085e4f200af4475b3690bd18) | Following commit adds xcNFT that is compliant with latest frame syntax and requirements | 
| 2.a | xcNFT Uniques |[Commit adding pallet_uniques compliant version of xcNFT](https://github.com/paraspell-research/xcnft-pallet/commit/447c7fc9bb84c47ab5a0f2171e4306270dfa67f5 ), [Current code](https://github.com/paraspell-research/xcnft-pallet/tree/main/xcnft-pallet_uniques) | Introduced pallet_uniques version of xcNFT | 
| 2.b | xcNFT NFTS |[Commit adding pallet_nfts compliant version of xcNFT](https://github.com/paraspell-research/xcnft-pallet/commit/99a1202fd258c5bc085e4f200af4475b3690bd18), [Current code](https://github.com/paraspell-research/xcnft-pallet/tree/main/xcnft-pallet_nfts) | Introduced pallet_nfts version of xcNFT | 
| 3 | xcNFT Abstract destination selection logic | [Commit adding abstracted destination logic to xcNFT pallet_nfts_version](https://github.com/paraspell-research/xcnft-pallet/commit/99a1202fd258c5bc085e4f200af4475b3690bd18), [Commit adding abstracted destination logic to xcNFT pallet_uniques version](https://github.com/paraspell-research/xcnft-pallet/commit/447c7fc9bb84c47ab5a0f2171e4306270dfa67f5)| Introduce abstracted destination selection logic in both versions of xcNFT (Users just enter Parachain ID)| 
| 4.a | xcNFT Burn asset |[Commit adding ability to burn collections or nfts cross-chain in xcNFT pallet_nfts version](https://github.com/paraspell-research/xcnft-pallet/commit/99a1202fd258c5bc085e4f200af4475b3690bd18), [Commit adding ability to burn collections or nfts cross-chain in xcNFT pallet_uniques version](https://github.com/paraspell-research/xcnft-pallet/commit/447c7fc9bb84c47ab5a0f2171e4306270dfa67f5)| Introduced cross-chain & pallet-agnostic collection or nft burn. | 
| 4.b | xcNFT Metadata |[Commit adding ability to update metadata for collections or nfts cross-chain in xcNFT pallet_nfts version](https://github.com/paraspell-research/xcnft-pallet/commit/99a1202fd258c5bc085e4f200af4475b3690bd18), [Commit adding ability to update metadata for collections or nfts cross-chain in xcNFT pallet_uniques version](https://github.com/paraspell-research/xcnft-pallet/commit/447c7fc9bb84c47ab5a0f2171e4306270dfa67f5)| Introduced cross-chain & pallet agnostic collection or nft metadata update. | 
| 4.c | xcNFT Transfer ownership | [Commit adding ability to change ownership for collections or nfts cross-chain in xcNFT pallet_nfts version](https://github.com/paraspell-research/xcnft-pallet/commit/99a1202fd258c5bc085e4f200af4475b3690bd18), [Commit adding ability to change ownership for collections or nfts cross-chain in xcNFT pallet_uniques version](https://github.com/paraspell-research/xcnft-pallet/commit/447c7fc9bb84c47ab5a0f2171e4306270dfa67f5)| Introduced cross-chain & pallet-agnostic collection or nft ownership transfer. | 
| 5. | xcNFT MultiAsset | [Commit adding ability to transfer collections with multiple NFTs cross-chain in xcNFT pallet_nfts version](https://github.com/paraspell-research/xcnft-pallet/commit/99a1202fd258c5bc085e4f200af4475b3690bd18), [Commit adding ability to transfer collections with multiple NFTs cross-chain in xcNFT pallet_uniques version](https://github.com/paraspell-research/xcnft-pallet/commit/447c7fc9bb84c47ab5a0f2171e4306270dfa67f5) | Introduced cross-chain pallet agnostic collection with multiple nfts transfer. | 

The provided commits no longer contain the latest version of xcNFT. There were some minor changes to certain functions since. The latest version is contained within [this commit](https://github.com/paraspell-research/xcnft-pallet/commit/e42b3aea8faa56760e02621d9bf6afc7f93c7279).

The pallet has to be tested within the [following repository](https://github.com/paraspell-research/polkadot-sdk) because the latest pallet_nfts and pallet_uniques update from the [following PR](https://github.com/paritytech/polkadot-sdk/pull/6087) hasn't yet been published.

**Additional Information**

Every aspect of the project, that was defined in the proposal, was implemented according to it. There were changes required during development - Some of the pallet_nfts and pallet_uniques structs were private to the pallet. This meant that we were unable to comply with the original frame pallets. We have opened PR requesting to change them from private to public so our pallet can comply - [PR Link](https://github.com/paritytech/polkadot-sdk/pull/6087). PR was **successfully merged**, so our xcNFT implementation is now **fully compliant** with the original frame pallet_nfts and pallet_uniques.