# Metacrafters_Assessment2
# Overview
## Contract Details
* tokenName: A public variable representing the name of the token.
* tokenAbbrv: A public variable representing the abbreviation or symbol of the token.
* totalSupply: A public variable representing the total supply of the token.
* balances: A mapping that stores the balance of each address holding the tokens.
### Constructor
The constructor initializes the contract with the provided token name, abbreviation, and initial supply.
It sets the totalSupply and assigns the entire initial supply to the address that deploys the contract.
### Mint Function
mint(address _to, uint256 _value) public: This function allows for the creation of new tokens.
It increases the total supply by the specified value and adds the same value to the balance of the specified address (_to).
### Burn Function
burn(address _from, uint256 _value) public: This function allows for the destruction of tokens.
It verifies that the sender has sufficient tokens to burn (balance is greater than or equal to the specified value).
It deducts the specified value from the total supply and the balance of the sender's address.
### Usage
* Deployment: Deploy the MyToken contract, providing the desired token name, abbreviation, and initial supply.
* Minting: Use the mint function to create new tokens and assign them to specific addresses.
* Burning: Use the burn function to destroy tokens, reducing the total supply and the balance of a specified address.
### Author
Patrick Nicolae M. Agbayani
