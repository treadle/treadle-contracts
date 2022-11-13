# treadle-contracts
This repository contains smart contracts of TREADLE Cycling App

# TRDLB contract
## To-Do List:
- [X] `nft_mint(received_id: AccountId, token_id: TokenId, metadata: TokenMetadata)` // owner only
- [X] `nft_token_metadata_edit(token_id: TokenId, metadata: TokenMetadata)` // owner only 

# Usage
## Building TRDLB smart contract
`./build.sh`

## Dev-deploying TRDLB smart contract
`near dev-deploy --wasmFile ./dist/trdlb.wasm`

## Initializing TRDLB contract with default metadata
`near call $NFT_CONTRACT_ID new_default_meta '{"owner_id": "'$YOUR_ACCOUNT_ID'"}' --accountId $YOUR_ACCOUNT_ID`

## Viewing TRDLB contract's metadata
`near view $NFT_CONTRACT_ID nft_metadata`
