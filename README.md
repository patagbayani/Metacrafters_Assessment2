## Public Variables
* tokenName: A public string variable representing the name of the token, set to "META".
* tokenAbbrv: A public string variable representing the abbreviation of the token, set to "MTA".
* totalSupply: A public unsigned integer variable representing the total supply of tokens, initially set to 0.
## Mapping
* balances: A mapping that associates an Ethereum address with a balance of tokens. Each address's balance is represented as an unsigned integer.
## Mint Function
** mint: A public function that allows for the creation of new tokens and distribution to a specified Ethereum address.
### Parameters:
* _address: The Ethereum address to which the new tokens will be assigned.
* _value: The number of tokens to create and assign to the specified address.
### Functionality:
* Increases the total supply of tokens by the specified value.
* Adds the specified value to the balance of the specified address.
## Burn Function
* burn: A public function that allows for the destruction (burning) of tokens from a specified Ethereum address.
### Parameters:
* _address: The Ethereum address from which tokens will be burned.
* _value: The number of tokens to burn from the specified address.
### Functionality:
Checks if the specified address has a sufficient balance to burn the specified value.
If the balance is sufficient, reduces the total supply by the specified value.
Reduces the balance of the specified address by the specified value.
