# Bid
[Git Source](https://github.com/Uniswap/twap-auction/blob/8cece7b4429d881c014ab2471e59a46f1e79e8cb/src/libraries/BidLib.sol)


```solidity
struct Bid {
    bool exactIn;
    uint64 startBlock;
    uint24 startCumulativeMps;
    uint64 exitedBlock;
    uint256 maxPrice;
    address owner;
    uint256 amount;
    uint256 tokensFilled;
}
```

