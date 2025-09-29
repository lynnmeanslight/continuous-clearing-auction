# IBidStorage
[Git Source](https://github.com/Uniswap/twap-auction/blob/8cece7b4429d881c014ab2471e59a46f1e79e8cb/src/interfaces/IBidStorage.sol)


## Functions
### nextBidId

Get the id of the next bid to be created


```solidity
function nextBidId() external view returns (uint256);
```

### bids

Get a bid from storage


```solidity
function bids(uint256 bidId) external view returns (Bid memory);
```

