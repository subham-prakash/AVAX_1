# Error Handling In Solidity

This smart contract provides functions to perform error handling using numbers. It demonstrates the usage of `require()`, `assert()`, and `revert()` statements in Solidity.

## Description
This program is a simple contract written in Solidity, a programming language used for developing smart contracts on the Ethereum blockchain. The contract has a three functions which we are used for performing the require(),revert() and assert() function to handles the error in solidity

## Getting Started

### Executing program

To run this program, you can use Remix, an online Solidity IDE. To get started, go to the Remix website at https://remix.ethereum.org/.

Once you are on the Remix website, create a new file by clicking on the "+" icon in the left-hand sidebar. Save the file with a .sol extension (e.g., ErrorHandling.sol). Copy and paste the following code into the file:

```javascript
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

contract ErrorHandlingContract {
    uint256 public num;

    function requireExample(uint256 _num) public {
        require(_num > 0, "Number must be greater than 0");
        
        num = _num;
    }

    function assertExample(uint256 _num) public {
        assert(_num != 0);
