### Execution Details

| Function           | Description                          | Transaction Hash                                                                 | Outcome                                      |
|--------------------|--------------------------------------|----------------------------------------------------------------------------------|----------------------------------------------|
| `setText`          | Changed message to "Hello from Abdullahi"         | `0xd1780607ebb153648ebff50f66c2a43b7c79187e85610381e3fb9caafe579d80`             | Success                                      |
| `transferOwnership`| Transferred ownership to `0xAb8483F64d9C6d1EcF9b849Ae677dD3315835cb2` | `0xfdc8a77c1856edb264aad64d30bb93fd1ad9009e422859137d6f62742fec0777` | Success, new owner confirmed                 |
| `setText (had to run this tx in remix vm since metamask was having diffuclties connecting)`          | Attempted invalid message as non-owner | `0x3afbb8d4a25a41b13ef31160c9e069a4f83ad5a769bd7318833863d5696953db` | Reverted: "Caller is not the owner"          |
| `transferOwnership (had to run this tx in remix vm since metamask was having diffuclties connecting)`| Attempted ownership transfer as non-owner | `0xaffff40e054c790707041d317371886920f0887df8a70e61935ae7e135596042` | Reverted: "Caller is not the owner"          |

**Contract Address**: `0x8c0E874d60E9108DD494675C4ad15E8dB14ca7fE`

**Previous Owner**: `0xAb38A5D4Feda8340A52803E60fCDd6a6E9cf8068`

**New Owner**: `0x9391be0ce59D66a64150cD466Dcd6577Db0C0329`
