# Solidity-101

## Introduction

Welcome! This is an automated workshop that will on using Solidity Smart contracts. It is aimed at developers who are not familiar with Solidity, or smart contracts.

## How to work on this TD

### Introduction

The workshop has two components:

- An ERC20 token, ticker `TD-SOL-101`, that is used to keep track of points
- A set of 15 exercises that are able to mint and distribute TD-SOL-101 points

Your objective is to gather as many TD-SOL-101 points as possible. Please note :

- You will need testnet Ether to do this workshop. Lookup "Sepolia testnet faucet" on google.
- The 'transfer' function of TD-SOL-101 has been disabled to encourage you to finish the TD with only one address

### Getting to work

- The instructions for each exercice are included in the contracts of each exercice, in [contracts/exercices](contracts/exercices).
- Each exercice contract inherits from the [exerciceTemplate](contracts/exerciceTemplate.sol), which holds common functions to validate students and credit points
- Each exercice is deployed on the Sepolia testnet. You can interact with them through [MyCrypto](https://mycrypto.com/contracts/interact), using the contract ABIs in [this folder](build/contracts), or through etherscan.
- In order to receive points, you will have to call function that execute code in each smart contract, such that the function `creditStudent(n, msg.sender);` is triggered, and distributes n points.
- A low level description of what is expected can be inferred by reading the code in each exercice.

## Exercises addresses

| Topic                                      | Contract code                                 | Contract on Etherscan                                                                   |
| ------------------------------------------ | --------------------------------------------- | --------------------------------------------------------------------------------------- |
| Points counter ERC20                       | [Points counter ERC20](contracts/TDERC20.sol) | [Link](https://sepolia.etherscan.io/address/0x2785f45160712657E91B62e106fE7Fc4bF6DC24c) |
| Calling a function                         | [Ex01](contracts/exercices/ex01.sol)          | [Link](https://sepolia.etherscan.io/address/0xD3BA7d92149E840F259EC54300e9410398E7CbC8) |
| Payable function                           | [Ex02](contracts/exercices/ex02.sol)          | [Link](https://sepolia.etherscan.io/address/0xFE036BC3aA74eF84C87131A78C18Ef378Cf77d59) |
| Requires                                   | [Ex03](contracts/exercices/ex03.sol)          | [Link](https://sepolia.etherscan.io/address/0x85A24203757D9e6494273796D07CC5Cbfc461031) |
| Storage variables                          | [Ex04](contracts/exercices/ex04.sol)          | [Link](https://sepolia.etherscan.io/address/0x16f95862578B6AF593D9748166a917e93fCb889B) |
| Mappings                                   | [Ex05](contracts/exercices/ex05.sol)          | [Link](https://sepolia.etherscan.io/address/0xE60D90d42013cF263757F0f4411A3ca0d36CF1D3) |
| Variable visibility                        | [Ex06](contracts/exercices/ex06.sol)          | [Link](https://sepolia.etherscan.io/address/0xb420246f7aFc4DBBDeF2aD4F13F9e281232B08c8) |
| Events                                     | [Ex07](contracts/exercices/ex07.sol)          | [Link](https://sepolia.etherscan.io/address/0x0011E72F249011311fd80Be3000515B815c71755) |
| Structures                                 | [Ex08](contracts/exercices/ex08.sol)          | [Link](https://sepolia.etherscan.io/address/0x6578782864eb582Fa7E284d9817915cCA4a5Bf02) |
| Code history                               | [Ex09](contracts/exercices/ex09.sol)          | [Link](https://sepolia.etherscan.io/address/0xe242F6A0069941dA40FAEB34E2Fa1eaf3Ca7AFA3) |
| Past transactions                          | [Ex10](contracts/exercices/ex10.sol)          | [Link](https://sepolia.etherscan.io/address/0x18f890776360d0136978D2a34f6846b634199E8C) |
| Composability                              | [Ex11](contracts/exercices/ex11.sol)          | [Link](https://sepolia.etherscan.io/address/0x02d2c498d063cB029f18F84EeA1Bb0d547585f39) |
| Blockchain forensics                       | [Ex12](contracts/exercices/ex12.sol)          | Undisclosed                                                                             |
| Deploy your contract to validate exercices | [Ex14](contracts/exercices/ex14.sol)          | [Link](https://sepolia.etherscan.io/address/0x4778169CEf44bF80407C3f87D444D4340AFee9ae) |
| All in one!                                | [Ex15](contracts/exercices/ex15.sol)          | [Link](https://sepolia.etherscan.io/address/0xC041afC6BD453E2Cd3b6f682c3F77358fFf9716e) |
