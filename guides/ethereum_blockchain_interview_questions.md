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

> A List Of Transactions, As Well As Uncles Is Incorporated In The Block. All Gas That Is Used During Those tTransactions Is Added To The Miners Balance. Also The Block Reward Is Added To The Miner, Then The Same Transactions Are Run Again By Every Participating Node In The Network To Achieve Consensus.

## Ethereum Programming Basics

`23. Smart Contracts Can Be Written In...`

> Solidity, Viper, LLL & Serpent As Those Are High-Level Languages That Are Compiled Down To Bytecode.

`24. Solidity Gets Compiled To...`

> Bytecodes - Essentially Opcodes Running Instruction By Instruction.

`25. Gas Is Used...`

> Depending On The Instruction/Opcode Run By The Ethereum Blockchain.

`26. To Store Almost All Data In The Ethereum Blockchain...`

> A Merkle Patricia Trie Is Used.

`27. You Interact With A Smart Contract & See A Gas Usage Of 50,000 With A Cost of 15Gwei. How Much Ether Would You Have To Pay To The Miner?`

> 750,000,000,000,000 Wei.

`28. Checking The Balance Of An Address Inside A Loop Of A Smart Contract Constantly...`

> Costs Gas Every Time We Check The Balance.

## Solidity Basics

`29. Solidity Files...`

> Can Be Spread Across Multiple Files. To Import All Contract From A File You Can Use “Import 'MyFile.Sol'. To Import Contract MyContract From MyFile.Sol You Use “Import {MyContract As SomeContract} From 'MyFile.Sol';”.

`30. Files Can Be...`

> Imported Using Relative & Absolute Paths, Where The “.” & The “..” Depict That It’s A Relative Path.

`31. Importing From GitHub...`

> Is Generally Possible, But Currently Works Only In Remix & Doesn’t Work In Truffle.

`32. Single Line Comments In Solidity Work With...`

> Either // Or ///.

`33. Multi-Line Comments In Solidity Work With...`

> With /* Comment */ Or /** @.. Natspec Style */

`34. The Following Are Value Types In Solidity...`

> Integer, Boolean, Enum & Addresses

`35. To Compare A String In Solidity You Use...`

> You Can’t Directly Compare Two Strings, But One Method Would Be To Hash Both Strings & Compare The Hashes.

`36. If We Divide Two Integers: 5/2, The Result Is...`

> 2 - Because The Decimal Is Truncated

`37. A Struct Is A Great Way...`

> To Define A New Datatype In Solidity, So You Don’t Need To Use Objects Of Another Contract.

`38. A Mapping Consists Of Keys & Value.`

> The Value Can Be Anything, But The Key Cannot Be Another Mapping, Struct, Enum Or Dynamically Sized Array.

`39. To Iterate Through A Mapping You...`

> Need An External Helper Variable.

`40. Function & Variable Visibility:`

> A Function Marked As Internal Can't Be Called By Other Contracts, Unless The Function Is Used By A Derived Contract. Private Functions Can't Be Called By Any Other Outside Contract & Public Variables Are Generating Automatically A Getter Function.

`41. View & Pure Functions:`

> A View Function Can Access State Variables, But Not Write To Them. A Pure Function Can't Modify Or Read From State.

`42. View & Pure Functions:`

> Can Be Accessed During Transactions & Calls.

`43. The Fallback Function:`

> Can Contain As Much Logic As You Want, But It’s Better To Keep It Short & Not Exceed The Gas Stipend Of 2,300 Gas.

`44. To Get The Address That Initiated The Transaction You Need To Use...`

> Tx.Origin.

`45. If I Call Contract A Which Calls Contract B, The Msg.Sender In Contract B Will Contain The Address of?`

> Contract A.

`46. Loops in Solidity...`

> Are Dangerous When Used With Data Structures That Grow Such As Arrays Or Mapping, Because It’s Hard To Estimate The Gas Requirements.

`47. Events:`

> Are Stored In Something Like A Side-Chain & Cannot Be Accessed By Contracts.

`48. According To The Official Style Guide...`

> Contract Names Should Be Capitalized, While Functions Should Be Mixed-Case. You Should Use 4 Spaces As Indentation & A Maximum Of 79 (Or 99) Characters Per Line.

`49. A Version Pragma Is A Great Way...`

> To Make It Clear For Which Compiler Version A Smart Contract Was Developed For. It Helps To Avoid Breaking Changes.

`50. Variables Of The Type Address Store...`

> A 20 Bytes Value.

## Ethereum Request For Comments

`51. What’s The Difference Between ERC & EIP?`

> Ethereum Request for Comments (ERC) Are Here To Define Standards For The Usage Of Ethereum. Ethereum Improvement Proposals (EIP) Are Here To Improve The Ethereum Protocol Itself.

`52. What Is The Difference Between ERC20 & ERC721 Tokens In Simple Terms?`

> The Tokens Of A Certain ERC-20 Symbol Are All The Same, The Tokens Of An ERC-721 Symbol Are All Different. So ERC-20 Tokens Are Fungible, While ERC-721 Tokens Are Non-Fungible.

`53. In Order To Implement An ERC20 Token Contract, You’d Need At Least To Implement The Following Functions & Events In Order To Fulfill The Interface Requirements:`

> totalSupply(), balanceOf(address), allowance(address, address), transfer(address, uint256), approve(address, uint256), transferFrom(address, address, uint256). Transfer(address, address, uint256), Approval(address, address, uint256).

## Solidity Advanced

`54. If Contract MyContractA Is Derived From Contract MyContractB, Then Which Would Be The Right Syntax:`

> Contract MyContractA Is MyContractB { … }.

`55. Inhertiance Is Useful, Because A Contract That Is Derived From Another Contract Can Make Use Of:`

> All Public State Variables & Properties, Public & Internal Functions & Modifiers.

`56. Finish The Sentence: The Library Web3.JS Is ...`

> Useful When Developing Distributed Applications With HTML & JavaScript, Because It Already Implements The Abstraction Of The JSON-RPC Interface Of Ethereum Nodes.

`57. When Solidity Is Compiled Then Also Metadata Is Generated.`

> The Metadata Contains The ABI Array, Which Defines The Interface To Interact With The Smart Contract. Metadata Can Also Contain The Address Of The Smart Contract When It Gets Deployed.

`58. The Difference Between address.send() & address.transfer() Is...`

> .send Returns A Boolean & .transfer Throws An Exception On Error. Both Just Forward The Gas-Stipend Of 2300 Gas & Are Considered Safe Against Re-Entrancy.

`59. All Low-Level Functions On The Address, So address.send(), address.call.value()(), address.callcode & address.delegatecall...`

> Return Booleans To Indicate An Error During Execution.

`60. When Using Assert To Check Invariants & It Evaluates To False...`

> All Gas Is Consumed.

`61. When Using Require To Check Input Parameters & It Evaluates To False...`

> All Remaining Gas Is Returned.

`62. To Send Ether To A Contract Without A Function Call:`

> A Fallback Function Must Be Declared & It Must Be Made Payable. If There Is No Fallback Function Or The Fallback Function Is Not Payable It Will Throw An Exception.

`63. Using selfdestruct(beneficiary) With The Beneficiary Being A Contract Without A Payable Fallback Function:`

> It’s Impossible To Secure A Contract Against Receiving Ether, Because selfdestruct Will Always Send Ether To The Address In The Argument. This Is A Design Decision Of The Ethereum Platform.

`64. If You Need More Fine-Grained Functionality Than Solidity Offers Out Of The Box...`

> You Can Incorporate Inline-Assembly To Get Better Controls.

`65. .Call vs. Delegatecall:`

> Address.call() Is Used For Calling Other Contracts Using The Scope Of The Called Contract In Terms Of Storage Variables. Address.delegatecall() Is Used For Libraries, Which Uses The Storage Variables Of The Contract Who Called. Libraries Are A Great Way To Re-Use Already Existing Code & delegatecall Can Make Sure That No Storage Is Used From The Library, Instead It Looks Like The Code Is Directly Copied Into The Calling Contract.

## Truffle & Ethereum Development Frameworks

`66. Truffle Is...`

> A Framework That Helps Developers With Testing, Deployment, Management Of Smart Contracts & Distributed Applications.

`67. Unit-Testing On A Local Chain Is Important, Because It Helps You Too...`

> Run Tests Quickly For Free, Compared To The Alternative Of Continuous Deployment On The Main-Network. This Saves You A Lot Of Fees, Time & Costs.

`68. With Truffle It's Easy To Write Clean-Room Unit-Tests For...`

> Solidity & Javascript

`69. With The Truffle Config File You Can Manage...`

> Different Networks To Deploy Your Contracts To. This Way You Can Easily Deploy To A Local Blockchain, The Main-Net Or The Ropsten/Rinkeby Test-Net With Only One Parameter.

