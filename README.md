
# Aptos Asset Template

## Overview

Aptos Asset Template is a project designed to provide a foundational framework for managing NFT assets and handling tokens on the Aptos blockchain. It includes sample implementations for creating, transferring, and managing digital assets.

## Features

-   **NFT Management**: Create, mint, and transfer NFTs.
    
-   **Token Processing**: Issue and manage fungible tokens.
    
-   **Asset Ownership**: Track and verify asset ownership securely on the blockchain.
    
-   **Metadata Support**: Store and retrieve metadata associated with NFTs.
    
-   **Smart Contract Templates**: Predefined Move modules for asset management.
    

## Requirements

-   [Aptos CLI](https://aptos.dev/cli-tools/aptos-cli/)
    
-   Move language knowledge
    
-   Rust (for Move compiler)
    
-   Aptos testnet or local network
    

## Installation

1.  Clone the repository:
    
    ```
    git clone https://github.com/thong847/aptos-asset-template.git
    cd aptos-asset-template
    ```
    
2.  Install dependencies:
    
    ```
    aptos init
    ```
    
3.  Compile the Move modules:
    
    ```
    aptos move compile
    ```
    
4.  Deploy to the Aptos blockchain:
    
    ```
    aptos move publish --profile default
    ```
    

## Usage

-   **Creating an NFT**:
    
    ```
    aptos move run --function-id default::nft::create --args <name> <description> <metadata_uri>
    ```
    
-   **Minting Tokens**:
    
    ```
    aptos move run --function-id default::token::mint --args <recipient_address> <amount>
    ```
    
-   **Transferring an NFT**:
    
    ```
    aptos move run --function-id default::nft::transfer --args <recipient_address> <nft_id>
    ```
    

## License

This project is open-source and available under the MIT License.
