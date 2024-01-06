# Blockchain Technologies 1  |  Bekbolat Karakuzov

## Overview
AITU_Bekbolat is an ERC-20 token built on the Ethereum blockchain. It is implemented using the OpenZeppelin library, which provides standard implementations of the ERC-20 interface.

## Usage

### Initial amount of tokens
```js
constructor() ERC20("AITU_Bekbolat", "UBQ") {
    _mint(msg.sender, 2000);
}
```

###  Functions

### getLatestTransactionTimestamp()
```js
function getLastTransactionTimestamp() external view returns (uint256) {
    return block.timestamp;
}
```

### getTransactionSender()
```js
function getTransactionSender() external view returns (address) {
    return msg.sender;
}
```

### getTransactionReceiver()
```js
function getTransactionReceiver() external view returns (address) {
    return address(this);
}

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [OpenZeppelin](https://openzeppelin.com/) for providing the ERC-20 implementation.
