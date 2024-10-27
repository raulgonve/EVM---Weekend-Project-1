Summary of all actions performed - 

1. Contract Deployment
Contract Deployment:
Transaction hash: 0xbfda79efc75b9be021bf33f387772dd1a16a3d56c1b1ac21fe994bcccad2f466
Block hash: 0xbe488c73079af22046db285e910a2cfbb6821606438a9f48f560994927246104
Contract address: 0xd9145CCE52D386f254917e481eB44e9943F39138


2. Set Text
Transaction hash: 0x7728e3518707234e6a69112c60ea9107e4f54b54ad42013b3d849e9725c2a046
Block hash: 0x0da325a7bc529ccf6496d463989b564abafcb35a26bb921ea4da4996d3544b69
0xd9145CCE52D386f254917e481eB44e9943F39138
Details: Changed the `text` of the contract from "Hello World" to "meow"

3. Ownership Transfer
Got a revert on original owner transfership attempt:

```
[vm]from: 0xAb8...35cb2to: HelloWorld.transferOwnership(address) 0xd91...39138value: 0 weidata: 0xf2f...35cb2logs: 0hash: 0x000...c6e31
transact to HelloWorld.transferOwnership errored: Error occurred: revert.

revert
	The transaction has been reverted to the initial state.
Reason provided by the contract: "Caller is not the owner".
If the transaction failed for not having enough gas, try increasing the gas limit gently.
```

Second Attempt at Transfer Attempt:
Transaction hash: 0xa9d04a53100ad1e50af0ee7933c7497aeccec1640a116849e874b48033664948
Block hash: 0x3312ddbaa65aac67fd6e2dffca5dae8904145b538270ac2626e9644fcbe35123
New owner input: {
	"address newOwner": "0xAb8483F64d9C6d1EcF9b849Ae677dD3315835cb2"
}