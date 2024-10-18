# Introduction to ETH and EVM

In eth mining happens via Proof of Stacke not via Proof of Wok(which it used to).

## Proof of stake
PoS in eth is a consensuse mechinism(alog for agreement in decentralized networks) that allows validators to create
and verify new blocks based on the amount of cryptocurrency they hold and are willing to "stake" as collateral.

# World State




# Evm Implementations
Any code that let's you start eth virtual mechine, is what is called an eth client. like for instence : ethereum/go-ethereum, ethereumproject/cpp-ethereum,

# Solidity ABIs, bytecode and opcode

Solidity is a high level programming language designed for writing smart contracts that run on the eth virtual machine.
When we swap one token to another, for ex: eth to usdc and when the that transaction initiated the $20 cut/taking in between/middle is smart contract.

When you compile solidity code, it will generate two thing for you 
1. Bytecode
2. ABIs

Bytecode -> Human-readable code converted into bytes. In the form of 0s & 1s. So bytes is solidity code is compiled.
And that Bytes is sequence of instructions(opcodes) taht can be understood and executed by the eth virtual machine.
Below is the simple solidity code, when we compile it will comple to bytes/hax.

```solidity
pragma solidity >=0.7.0 <0.9.0;

contract Counter {
    uint256 private count;

    constructor() {
        count = 0;
    }

    function upWardCount() public {
        count += 1;
    }

    function downWardCount() public {
        require(count > 0, "Count cannot go below then this.");
        count -= 1;
    }
}
```
# Opcode
An opcode is the first byte of an instruction in machine language which tells the hardware what operation needs to be performed with this instruction. Every processor/controller has its own set of opcodes defined in its architecture.  An opcode is followed by data like address, values etc if needed.

# ABIs (application binary interface)
It's is like saying what does the interface look like, and how can I talk to the smart contract/intaract. and also what function exists in this smart contract.
























## Class Project 
-  Wallet adapters in ETH
-  Eth on the server, etherjs
-  Eth with React and Next.js
