# Weekend Project: HelloWorld.sol Interaction

This project is part of the EVM-Bootcamp weekend challenge. The objective is to collaboratively interact with the **HelloWorld.sol** contract to modify the message (`text` variable) and transfer contract ownership. Each function execution, along with the transaction hash or revert reason, will be documented.

## Project Overview

The **HelloWorld.sol** smart contract provides the following functionalities:
- View the current message (`helloWorld` function).
- Set a new message (`setText` function) – restricted to the contract owner.
- Transfer contract ownership (`transferOwnership` function) – restricted to the contract owner.

Our group has explored these functionalities and documented all interactions, including transaction outcomes and any encountered errors.

## Team Members
- Raul Gonzalez - k2NaNm - @Cryptowolf 
- kNohaF    - @LucasRohr 
- AvgRax    - @Meet
- Marguerite Blair - XEGTvv    - @eratosthenessieve 
- crg7DC - @hagi 
- Esteban Valsecchi - YNgtg8 - @Esteban CryptoBull13 
- JDxvP6    - @Vamshi

## Contract Functions

### `helloWorld()`
- **Description**: Returns the current message text stored in the contract.
- **Access**: Public, view only.

### `setText(string calldata newText)`
- **Description**: Allows the owner to set a new message.
- **Access**: Restricted to the contract owner (via `onlyOwner` modifier).
- **Error Handling**: Reverts with "Caller is not the owner" if called by a non-owner.

### `transferOwnership(address newOwner)`
- **Description**: Allows the owner to transfer contract ownership to a new address.
- **Access**: Restricted to the contract owner (via `onlyOwner` modifier).
- **Error Handling**: Reverts with "Caller is not the owner" if called by a non-owner.

## Interaction Steps

1. **Connect to Contract**  
   We connected to the **HelloWorld.sol** contract deployed on [Network Name].

2. **Set Message**  
   Each group member, while connected as the owner, interacted with the contract to set a new message using `setText`.

3. **Transfer Ownership**  
   Ownership transfer functionality was tested among group members using `transferOwnership`.

## Execution Details

| Function           | Description                     | Transaction Hash                          | Outcome               |
|--------------------|---------------------------------|-------------------------------------------|-----------------------|
| `setText`          | Changed message to "Hello!"     | `0x1234abcd...`                           | Success               |
| `transferOwnership`| Transferred ownership to [Name] | `0xabcd1234...`                           | Success               |
| `setText`          | Attempted invalid message       | N/A                                       | Reverted: "Caller is not the owner" |

> **Note:** Full interaction logs are provided in the attached report.

## Submission

To submit, we will complete the provided form in Discord with all required documentation, including our report and GitHub repository link.

---