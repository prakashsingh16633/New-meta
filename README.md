MyToken Contract
Description
The MyToken contract is a simple implementation of a token on the Ethereum blockchain. It allows for the creation (minting) and destruction (burning) of tokens, as well as querying token balances.

Requirements
Token Details: The contract stores details about the token, including its name, abbreviation, and total supply.
Balances Mapping: The contract maintains a mapping of addresses to token balances.
Mint Function: A function to create new tokens (mint) by increasing the total supply and adding to the balance of a specified address.
Burn Function: A function to destroy tokens (burn) by reducing the total supply and deducting from the balance of a specified address. This function includes conditional checks to ensure the sender has sufficient balance to burn.
Usage
Deploy Contract: Deploy the MyToken contract to the Ethereum blockchain.
Mint Tokens: Call the mint function, providing the address to receive tokens and the amount to mint.
Burn Tokens: Call the burn function, providing the address of the tokens to burn and the amount to burn.
Example
solidity
Copy code
// Deploy contract
MyToken token = new MyToken();

// Mint tokens
token.mint(addressToReceiveTokens, amountToMint);

// Burn tokens
token.burn(addressToBurnTokens, amountToBurn);
