# DemandLib
[Git Source](https://github.com/Uniswap/twap-auction/blob/8cece7b4429d881c014ab2471e59a46f1e79e8cb/src/libraries/DemandLib.sol)

Library for demand calculations and operations


## Functions
### resolve

Resolve the demand at a given price

*"Resolving" means converting all demand into token terms, which requires dividing the currency demand by a price*


```solidity
function resolve(Demand memory _demand, uint256 price) internal pure returns (ValueX7);
```
**Parameters**

|Name|Type|Description|
|----|----|-----------|
|`_demand`|`Demand`|The demand to resolve|
|`price`|`uint256`|The price to resolve the demand at|

**Returns**

|Name|Type|Description|
|----|----|-----------|
|`<none>`|`ValueX7`|The resolved demand as a ValueX7|


### _resolveCurrencyDemand

Resolve the currency demand at a given price


```solidity
function _resolveCurrencyDemand(ValueX7 amount, uint256 price) private pure returns (ValueX7);
```

### add


```solidity
function add(Demand memory _demand, Demand memory _other) internal pure returns (Demand memory);
```

### sub


```solidity
function sub(Demand memory _demand, Demand memory _other) internal pure returns (Demand memory);
```

### scaleByMps

Apply mps to a Demand struct

*Shorthand for calling `scaleByMps` on both currencyDemandX7 and tokenDemandX7*


```solidity
function scaleByMps(Demand memory _demand, uint24 mps) internal pure returns (Demand memory);
```

