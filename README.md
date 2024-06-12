We start by declaring the version of Solidity we are using and the license of the contract.
Next, we define our contract named MyToken. We declare three public variables: name, symbol, and totalSupply. 
These will store the token's name, its abbreviation, and the total supply of tokens respectively.We then create a mapping to store the balance of each address. 
This mapping is called balances and it maps an address to a uint, which represents the balance of that address."Here is our mint function. 
This function takes an address and a value as parameters. It increases the totalSupply by the given value and also increases the balance of the specified address by the same amount. 
Finally, it emits a Mint event.Next, we have the burn function. This function also takes an address and a value as parameters.
It first checks if the balance of the given address is greater than or equal to the value to be burned using the require statement. 
If this condition is met, it decreases the totalSupply and the balance of the specified address by the given value. It also emits a Burn event.
