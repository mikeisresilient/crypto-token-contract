

# MyToken (Psyche)

A simple ERC20-style token smart contract written in Solidity. This contract allows you to create, transfer, and manage tokens on Ethereum-compatible networks.

## Token Details

| Property     | Value             |
| ------------ | ----------------- |
| Name         | MyToken           |
| Symbol       | Psyche            |
| Decimals     | 18                |
| Total Supply | Set at deployment |

## Features

* Standard ERC20 functionality:

  * `transfer`: Send tokens to another address
  * `approve`: Allow an address to spend tokens on your behalf
  * `transferFrom`: Transfer tokens using an approved allowance
* Track balances and allowances
* Emits `Transfer` and `Approval` events for transparency

## Deployment

1. Use [Remix IDE](https://remix.ethereum.org/) or a local development framework like [Hardhat](https://hardhat.org/).
2. Copy the `MyToken.sol` contract into a new Solidity file.
3. Compile the contract with Solidity version `^0.8.0`.
4. Deploy the contract and specify the initial supply (e.g., `1000000` for 1 million tokens).
5. The deployer address receives the full initial supply.

## Usage

* **Transfer tokens**

```solidity
token.transfer(recipientAddress, amount);
```

* **Approve allowance**

```solidity
token.approve(spenderAddress, amount);
```

* **Transfer tokens using allowance**

```solidity
token.transferFrom(ownerAddress, recipientAddress, amount);
```

## Events

* `Transfer(address indexed from, address indexed to, uint256 value)` – emitted on token transfers
* `Approval(address indexed owner, address indexed spender, uint256 value)` – emitted when setting an allowance

## License

This project is licensed under the MIT License.
