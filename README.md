## Introduction

Solidity is the primary language for developing smart contracts on blockchain platforms like Celo. One exciting use case of smart contracts is to implement decentralized games such as a lottery. This challenge focuses on creating a simple lottery contract in Solidity.

## Problem Statement

Design a smart contract that simulates a simple lottery with the following requirements:

1. The contract should allow users to buy lottery tickets by sending a certain amount of Celo (to be specified by you).
2. Each time a user buys a ticket, the user's address is added to a pool of participants.
3. The contract should include a function that chooses a random winner from the pool of participants.
4. Only the contract owner should be allowed to call the function that chooses the winner.
5. When a winner is chosen, the entire balance of the contract should be transferred to the winner, and the pool of participants should be reset.

## Hints

- Use a dynamic array to store the pool of participants.
- To generate a random number, consider using the hash of the current block number and timestamp.
- Use `msg.sender` and `msg.value` to handle the purchase of tickets.
- Use a `require` statement to enforce that only the contract owner can pick the winner.
- The `transfer` function can be used to send the contract's balance to the winner.

## Evaluation Criteria

- **Correctness**: The contract should compile without errors and fulfill all the requirements.
- **Readability**: The contract should be well-documented, with comments explaining the code.
- **Testability**: You should also provide examples of how to test each function of the contract.

Please note that generating truly random numbers in a deterministic system like Ethereum or Celo is a complex issue, and the method suggested here is not suitable for high-stakes lottery games.

For a comprehensive understanding of Celo smart contracts and Solidity, please refer to the Celo and Solidity tutorials.

## Submission

Please reply with a link to your PR on GitHub, including your lottery contract. Also, include any notes or comments you think are necessary to understand your design and choices. Lastly, provide a brief explanation about how each function of the contract should be tested.
