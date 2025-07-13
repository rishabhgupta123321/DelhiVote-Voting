# DelhiVote
A decentralized voting smart contract for ETHGlobal New Delhi 2025.

## Overview
As a Solidity beginner, I built DelhiVote to explore Web3 governance, using a voting template from Solidity by Example. I studied the code to understand structs, mappings, and user interactions, customized the contract name and proposals, and deployed it on Sepolia for ETHGlobal.

## Deployment
- **Network**: Sepolia Testnet
- **Contract Address**: [https://sepolia.etherscan.io/address/0xd751cea6971bc0e213aed278ef6dfba49fce412c](https://sepolia.etherscan.io/address/0xd751cea6971bc0e213aed278ef6dfba49fce412c)

## Features
- **Proposals**: Predefined options ("Proposal A", "Proposal B").
- **Voting**: Users vote once for a proposal, tracked to prevent double-voting.
- **Result**: View the winning proposal with the highest votes.
- **Security**: Uses safe math (Solidity ^0.8.20) and input validation.

## Code Breakdown
`DelhiVote.sol` implements a voting system:                                                 
- **Constructor**: Initializes the owner and two proposals ("Proposal A", "Proposal B").
- **Vote**: Allows one vote per user, tracked via a `voters` mapping, and emits a `Voted` event.
- **GetWinningProposal**: Returns the proposal with the most votes by iterating through a `Proposal` struct array.
- **Security**: Uses `require` to prevent double-voting and invalid proposals.

I learned how structs organize data, mappings track user actions, and loops determine results. Deploying via Remix was a smooth experience.

## Files
- **`DelhiVote.sol`**: Defines the voting contract.
- **`LICENSE`**: MIT License, allowing open-source use.
- **`.gitignore`**: Node.js template with `artifacts/` for clean commits.
- **`README.md`**: This file, detailing my project and journey.

## Source
Built using [Solidity by Example’s voting template](https://docs.soliditylang.org/en/latest/solidity-by-example.html#voting), licensed under MIT. I customized the contract name and proposals while learning from the code.
  
## My Journey
Building DelhiVote was an exciting leap into Web3 governance! Studying the contract taught me about data structures and user interaction in Solidity. Deploying to Sepolia and verifying on Etherscan was a proud moment. I named it “DelhiVote” to celebrate my journey toward ETHGlobal New Delhi 2025.

## Usage
- Compile and deploy `DelhiVote.sol` in Remix (Solidity 0.8.20).
- Vote for a proposal via MetaMask or ethers.js.
- Check the winning proposal using `getWinningProposal`.
- Verify on Etherscan.

## License
Licensed under the MIT License—see [LICENSE](LICENSE).

## Contact
Email me at rishabhgupta78470@gmail.com or find me on X @rishabh_guptaz. Excited to connect at ETHGlobal New Delhi 2025!
