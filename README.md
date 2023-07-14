# ETH-AVX-Module3

CustomToken Contract

License
This contract is using the MIT License.

Prerequisites
Solidity ^0.8.9

Contract Details:
The contract imports three contracts from the OpenZeppelin library:

ERC20: This is the standard ERC20 token contract implementation, providing basic functionality for a fungible token.
ERC20Burnable: This contract extends ERC20 and adds the ability to burn (destroy) tokens.
Ownable: This contract provides a basic access control mechanism, allowing only the contract owner to execute certain functions.
The CustomToken contract is defined and inherits from ERC20, ERC20Burnable, and Ownable.

The constructor function is defined without any parameters. It is executed once when the contract is deployed. Within the constructor, the ERC20 constructor is called with the name "MyToken" and symbol "MyTk" to initialize the token.

The mint function is a public function that can only be called by the contract owner (as defined by the Ownable contract). It takes two parameters: to (the address to which the tokens will be minted) and amount (the number of tokens to mint). Inside the function, the _mint function from the ERC20 contract is called to create and assign the specified amount of tokens to the given address.

Video Walkthrough
https://www.loom.com/share/fd0387abfc944c4491023ca8bc2d1871
