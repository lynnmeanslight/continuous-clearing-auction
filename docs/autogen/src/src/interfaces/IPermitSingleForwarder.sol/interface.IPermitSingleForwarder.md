# IPermitSingleForwarder
[Git Source](https://github.com/Uniswap/twap-auction/blob/8cece7b4429d881c014ab2471e59a46f1e79e8cb/src/interfaces/IPermitSingleForwarder.sol)

Interface for the PermitSingleForwarder contract


## Functions
### permit

allows forwarding a single permit to permit2

*this function is payable to allow multicall with NATIVE based actions*


```solidity
function permit(address owner, IAllowanceTransfer.PermitSingle calldata permitSingle, bytes calldata signature)
    external
    payable
    returns (bytes memory err);
```
**Parameters**

|Name|Type|Description|
|----|----|-----------|
|`owner`|`address`|the owner of the tokens|
|`permitSingle`|`IAllowanceTransfer.PermitSingle`|the permit data|
|`signature`|`bytes`|the signature of the permit; abi.encodePacked(r, s, v)|

**Returns**

|Name|Type|Description|
|----|----|-----------|
|`err`|`bytes`|the error returned by a reverting permit call, empty if successful|


