# treadle-contracts
This repository contains smart contracts of TREADLE Cycling App

# TRDLB contract
## To-Do List:
- [X] nft_mint(...);
- [X] nft_metadata_edit(token_id: TokenId, metadata: TokenMetadata); 
- [ ] nft_burn(token_id: TokenId);

# Usage
## Building a smart contract
`./build.sh`

## Dev-deploying the smart contract
`near dev-deploy --wasmFile ./dist/trdlb.wasm`

## Initializing the contract with default metadata
`near call $NFT_CONTRACT_ID new_default_meta '{"owner_id": "'$YOUR_ACCOUNT_ID'"}' --accountId $YOUR_ACCOUNT_ID`

## Viewing the contract's metadata
`near view $NFT_CONTRACT_ID nft_metadata`
