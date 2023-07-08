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

Now the detailed explanations for the mapping and conditional statement used in the code:

Mapping:

- The "mapping" keyword is used to define a data structure that maps one type of data to another. In this code, the "balances" variable is a mapping that maps addresses to 
  their respective token balances. The "address" type is used as the key for the mapping, and the "uint" type is used as the value.

- The "public" keyword before the "balances" variable makes it accessible from outside the contract and generates a getter function automatically. This allows anyone to 
  check the balance of any address by calling the "balances" mapping with the desired address as the input.

Conditional statement:

- The "if" statement is a conditional statement that executes a block of code only if a certain condition is true. In this code, the "burn" function includes an "if" 
  statement that checks if the balance of the specified address is greater than or equal to the value being burned. If the condition is true, the code inside the "if" block 
  will be executed, which subtracts the value from the total supply and from the balance of the specified address.

- The ">= operator" checks if the balance is greater than or equal to the value being burned. If the balance is equal to the value being burned, the balance will become 
  zero after the "burn" function is called. If the balance is less than the value being burned, the "if" block will not be executed, and the balance and total supply will 
  remain unchanged.
