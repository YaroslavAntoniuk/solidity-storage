# Solidity Storage Contracts

This project contains three Solidity contracts that demonstrate different ways to store data on the Ethereum blockchain.

## SimpleStorage.sol

This contract provides a simple way to store a favorite number and a mapping of names to favorite numbers. It also allows for the addition of people, each with a favorite number and a name. The `store` function is used to store a favorite number, and the `retrieve` function is used to get the stored favorite number. The `addPerson` function is used to add a person with a name and a favorite number.

## StorageFactory.sol

This contract creates instances of the SimpleStorage contract. It maintains an array of these instances. The `createSimpleStorage` function is used to create a new SimpleStorage contract and add it to the array. The `sfStore` function is used to store a number in a specific SimpleStorage contract in the array. The `sfGet` function is used to retrieve the stored number from a specific SimpleStorage contract in the array.

## ExtraStorage.sol

This contract extends the SimpleStorage contract and overrides the `store` function. When a number is stored using this contract, 5 is added to it before it is stored. This demonstrates how contract inheritance and function overriding work in Solidity.
