# User FAQs

If you have a question that isn't answered here, please contact us in [our Discord](https://discord.gg/blockscout) and the team and community can help troubleshoot your issue.

## User FAQs

<details>

<summary>What does the "in" or "out" label mean on a transaction?</summary>

This label appears next to a transaction to signify whether a transaction was sent or received by a particular address.

* <mark style="color:green;background-color:green;">**In**</mark>**:** A transaction was sent to the address
* <mark style="color:orange;background-color:orange;">**Out**</mark>**:** A transaction was initiated from the address

<img src="../.gitbook/assets/tx1.png" alt="" data-size="original">

</details>

<details>

<summary>What are the different transaction types?</summary>

**There are 3 transaction types which can be accessed from the tabs menu for an EOA (Externally Owned Address) or Smart Contract.**

**Transactions:**\
An EOA, commonly known as a wallet address, initiates a transaction. Both incoming and outgoing transactions are recorded here, and includes any transaction that requires a gas fee (in the native token ETH, xDai etc) for execution.

**Token Transfers:**\
Transactions of ERC-20 or ERC-721 tokens. This can include DeFi transactions (like adding or removing liquidity), EOA transfers, airdrops or other transactions where non-native tokens are sent and received.

**Internal Transactions:**\
Transactions initiated and executed between smart contracts. Internal transactions are the result of an external transaction (EOA to contract). This initial transaction can then trigger many internal transactions between contracts as functions are called.

<img src="../.gitbook/assets/tokens-tab.png" alt="" data-size="original">

</details>

<details>

<summary>What is CSV export error 504?</summary>

If you request too much data at the same time you may receive a timeout. Decreasing the period of time for an export (**1 week timeframe** is recommended for addresses with lots of transactions) can reduce these errors.

</details>

<details>

<summary>How can I access and read/write contract methods?</summary>

Yes! The contract should be verified (or the bytecode matches an existing contract) to enable reading and writing to contracts and proxy contracts. [More info here](../developer-support/smart-contract-verification/interacting-with-smart-contracts.md).

</details>

<details>

<summary>How do I verify a smart contract?</summary>

There are multiple methods including options from the Blockscout UI as well as an integration directly with Hardhat.

**Blockscout UI:**

* [Via flattened source code (Solidity)](../developer-support/smart-contract-verification/#via-flattened-source-code)
* [Via standard JSON input](faqs.md#via-standard-json-input)
* [Via Sourcify: Sources and metadata JSON file](../developer-support/smart-contract-verification/contracts-verification-via-sourcify.md)
* [Vyper contract](../developer-support/smart-contract-verification/#vyper-contract)

**Hardhat:**

* [Hardhat Verification Plugin](../developer-support/smart-contract-verification/hardhat-verification-plugin/)
* [Sourcify Plugin for Hardhat](../developer-support/smart-contract-verification/hardhat-verification-plugin/sourcify-plugin-for-hardhat.md)

</details>
