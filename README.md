# MappingStorage.sol
How to deploy a contract on Base Chain MappingStorage.sol
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract MappingStorage {
    mapping(address => uint) public balances;

    function setBalance(uint _amount) public {
        balances[msg.sender] = _amount;
    }
}
