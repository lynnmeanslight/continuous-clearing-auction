# Demand
[Git Source](https://github.com/Uniswap/twap-auction/blob/8cece7b4429d881c014ab2471e59a46f1e79e8cb/src/libraries/DemandLib.sol)

Struct containing currency demand and token demand

*All values are in ValueX7 format*


```solidity
struct Demand {
    ValueX7 currencyDemandX7;
    ValueX7 tokenDemandX7;
}
```

