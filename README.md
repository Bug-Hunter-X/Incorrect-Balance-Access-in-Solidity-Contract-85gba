# Incorrect Balance Access in Solidity Contract

This repository demonstrates a common error in Solidity smart contracts: incorrect access to the balance of an account.

The `balanceOf` function incorrectly accesses the `balances` mapping instead of using the correctly named `balanceOf` mapping.

## Bug
The provided Solidity code contains an error in the `balanceOf` function. It attempts to read the balance from a mapping named `balances`, which likely doesn't exist, leading to an unexpected behavior or runtime error. The correct mapping to use is `balanceOf`.

## Solution
The solution involves correcting the access to the balance mapping in the `balanceOf` function. By using the correctly named mapping, the function will now correctly return the account balance.
