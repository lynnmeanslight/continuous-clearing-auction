# Bid
[Git Source](https://github.com/Uniswap/twap-auction/blob/e1dbf4f02e1bcbb91486a39f0f49eb2aeb52ecc6/src/libraries/BidLib.sol)


```solidity
struct Bid {
    bool exactIn;
    uint64 startBlock;
    uint64 exitedBlock;
    uint256 maxPrice;
    address owner;
    uint128 amount;
    uint128 tokensFilled;
}
```

