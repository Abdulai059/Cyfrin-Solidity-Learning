# Name to Favorite Number Mapping

This is a simple Solidity smart contract that demonstrates a mapping from names (represented as `string`) to favorite numbers (represented as `uint256`). The contract stores favorite numbers associated with a name and makes this data publicly accessible on the blockchain.

## Smart Contract Overview

The main functionality is to store and retrieve a person's favorite number based on their name.

### Code Snippet

```solidity
mapping(string => uint256) public nameTofavoriteNumber;
```

- `nameTofavoriteNumber`: A `mapping` where each `string` (name) key maps to a `uint256` (favorite number) value. This mapping is `public`, allowing for easy access to the favorite number associated with any given name.

## Usage

1. **Store a Favorite Number**: A function (not shown in the snippet) would allow users to associate a favorite number with a given name.
2. **Retrieve a Favorite Number**: Since `nameTofavoriteNumber` is public, you can access a favorite number directly by querying the mapping with a name.

Example usage:

```solidity
// Assuming the name "Alice" has a favorite number of 42
uint256 aliceFavoriteNumber = nameTofavoriteNumber["Alice"];
```

## Requirements

- Solidity version ^0.8.0
- An Ethereum-compatible development environment (such as Remix or Hardhat)

## Deployment

You can deploy this contract on Ethereum-compatible networks or local test environments like Ganache or Hardhat.

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.
