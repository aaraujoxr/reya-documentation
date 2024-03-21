# Margin accounts

Users can create multiple accounts per wallet, where each account is represented as an ERC-721 Token. This provides users with the ability to create segregated accounts for trades they don’t want cross-margined with other positions. The use of an ERC-721 Token also provides the following benefits:

* Users can transfer these accounts to another wallet without unwinding any positions. In many ways, this is akin to in-specie transfers and provides a significant improvement in functionality for sophisticated actors on the protocol.
* Segregated account owners, which can be EOAs or smart contracts, are able to prescribe granular permissioning rules to other EOA and smart contract addresses. This may, for example, allow a user to have a cold wallet for withdrawals but grant permissions to their hot wallet to conduct trades without giving it withdrawal access
* Since addresses are decoupled from accounts, it is possible to layer in further abstractions that govern delegation and authorization flows improving account management operational security.
