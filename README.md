# Project Title

MyToken Contract.

## Description

The MyToken contract is a simple token on the Ethereum blockchain. It can create new tokens (mint) and destroy existing ones (burn). The contract keeps track of the total supply of tokens and the balances of each address.

## Getting Started

### Installing

To use this contract, we will need:
- An Ethereum development environment like [Remix IDE](https://remix.ethereum.org/).

### Executing program

To deploy and interact with the MyToken contract, follow these steps:

1. **Open Remix IDE or your preferred Ethereum development environment.**
2. **Create a new file and paste the contract code**
3. **Compile the contract.**
4. **Deploy the contract to your desired Ethereum network.**
5. **Interact with the contract using the deployed contract's interface:**
    - To mint tokens, call the `mint` function with the address and the amount to mint:
      
      function mint(address _adrs , uint _value) public {
        totalSupply += _value;
        balances[_adrs] += _value;
    }

      
    - To burn tokens, call the `burn` function with the address and the amount to burn:
      
       function burn(address _adrs , uint _value) public {

        if (balances[_adrs] >= _value) {
            totalSupply -= _value;
            balances[_adrs] -= _value;

        }

    }

  
### Help

- Ensure that your Ethereum node or provider is running and properly connected.
- Verify that the address provided for minting or burning has the appropriate balance.


## Authors

- **Akash Kumar Singh**
  - GitHub: [GitHubHandle](https://github.com/Akash-Kumar-Singh786/ETH-PROOF-Beginner-EVM-Course-final-assessment/tree/main)
  - Email: [email](akashkumarsingh203@gmail.com)

## License

This project is licensed under the MIT License - for details see the LICENSE.md file .
