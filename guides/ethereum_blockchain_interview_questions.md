# Ethereum Blockchain Interview Questions

## Ethereum & EVM Basics

`1. Which Is The Right Order Of Denominations?`

> Wei, Finney, Ether & Tether.

`2. A Transaction Contains the Nonce Field. Why?`

> To Avoid Replay Attacks.

`3. What Is The Nonce-Field In A Transaction For?`

> To Protect Against Replay Attacks.

`4. The EVM Can’t Access Hardware Layers, Or Anything Outside A Blockchain Node As It’s Sandboxed.`

> True.

`5. Decentralised Applications...`

> Cut Out The Middle-Man, Run On A Trusted Platform, Apply Logic To The Blockchain Where Economic Assets Are Already Running Thus Allowing Peer-To-Peer Transactions.

`6. To Get The Most Out Of The Blockchain It Is Best...`

> To Use It Only For Those Things Which Need The Capabilities Of A Blockchain.

`7. What Does It Mean When A Hashing Algorithm Is Deterministic?`

> Given The Same Input It Will Always Produce The Same Output.

`8. 1 Ether = 10^18 Wei, 10^9 Gwei, 10^3 Finney`

> Correct.

`9. What Are Private Keys For?`

> To Sign Transactions & Derive Addresses From.

`10. Private Keys Sign Transactions & Public Keys Verify Signatures`

> True.

`11. Proof Of Work (PoW) VS. Proof Of Stake (PoS)`

> PoW Is Computationally Intensive Which Requires A Lot Of Energy. PoS Miners Earn A Straightforward Reward For Mining A Block & Incorporating Transactions.

`12. Externally Owned Accounts...`

> Are Bound To A Private Key Which Is Necessary To Sign Transactions Outgoing From That Account.

## Ethereum Nodes & Networks

`13. What Are Ethereum Nodes?`

> Programs Implementing The Ethereum Protocol To Talk To Each Other, & JSON-RPC Interfaces To Talk To The Outside World.

`14. To Communicate With An Ethereum Node Via JavaScript...`

> The Library You Use Must Make Use Of The JSON-RPC Interface Of An Ethereum Node.

`15. It’s Possible To Access The Blockchain Via An Ethereum Node`

> By Any Programming Language As Long As It Adheres To The JSON-RPC Standard

`16. A Private Network Is...`

> A Network Running Only In A Private Area Where People Cannot Join Freely & Openly.

`17. For Rapid Development Cycles It’s Good...`

> To Use In-Memory Blockchain Simulations, Because Mining Works Instantaneously.

`18. Go-Ethereum VS. Ganache`

> With Go-Ethereum You Get A Real Blockchain Node Where You Can Create Your Own Local Private Network, Connect To Test-Networks Or The Main-Net, While With Ganache You Get An In-Memory Blockchain Simulation.

`19. Block Timestamp...`

> The Timestamp Can Be Influenced By A Miner To A Certain Degree, But It’s Always Independent From The Time-Zone.

`20. Block Difficulty...`

> The Block Difficulty Increases When The Time Between Mined Blocks Is Below 10 seconds, While It Decreases When The Time Is Above 20 Seconds.

`21. Ethereum Nodes...`

> Must Implement The Ethereum Protocol & A JSON-RPC To Talk With Clients.

`22. When A New Block Is Mined...`

> A list Of Transactions, As Well As Uncles Is Incorporated In The Block. All Gas That Is Used During Those tTransactions Is Added To The Miners Balance. Also The Block Reward Is Added To The Miner, Then The Same Transactions Are Run Again By Every Participating Node In The Network To Achieve Consensus.
