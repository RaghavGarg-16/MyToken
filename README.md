# MyToken
This is my Solidity code for a simple token contract with the following variables and functions:

Variables:

- tokenName: a public string variable representing the name of the token.
- tokenAbbry: a public string variable representing the abbreviation of the token.
- totalSupply: a public uint variable representing the total supply of the token.
- balances: a public mapping variable that maps the balance of an address to a uint.

Functions:

- mint: a public function that adds to the total supply and increases the balance of a specified address.
- burn: a public function that subtracts from the total supply and decreases the balance of a specified address, only if the balance is greater than the value being burned.
