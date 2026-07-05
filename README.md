# TON Onboarding Challenge

TypeScript and FunC work for the TON onboarding proof-of-work NFT challenge. The project explores how a TON smart-contract workflow is structured, tested, and executed locally before interacting with the network.

This repository is based on the official TON onboarding challenge and keeps the original learning goal: understand the proof-of-work minting flow by working through the contract and TypeScript tooling.

## What it covers

- TON smart-contract project layout
- FunC source files for collection and NFT item logic
- TypeScript wrappers for code and data cells
- Local contract interaction helpers
- Jest tests for giver and item behavior
- Proof-of-work mining flow concepts
- QR-code / wallet interaction tooling from the challenge boilerplate

## Tech stack

- TypeScript
- FunC
- TON libraries
- Jest
- Yarn

## Install

```bash
yarn install
```

## Run

```bash
yarn start
```

## Tests

```bash
yarn jest
```

## Repository structure

```text
index.ts            Main script entrypoint
src/func/           FunC contract sources
src/giver/          NFT giver code, data, tests, and local wrapper
src/item/           NFT item code, data, tests, and local wrapper
src/lib/            Shared utilities
jest.config.js      Jest setup
tsconfig.json       TypeScript config
```

## Challenge idea

The onboarding challenge uses a proof-of-work style minting flow. A miner searches for proof data that satisfies the current contract difficulty, then sends the valid proof in an internal message to mint the NFT reward.

That makes the project useful for learning:

- how TON cells are structured
- how contract state is read through get-methods
- how proof data is assembled
- how TypeScript tooling supports smart-contract work

## Official references

- [TON Onboarding Challenge](https://ton.org/docs/develop/onboarding-challenge)
- [Video tutorial](https://youtu.be/wEEQLwQy30Q)

## Technical highlights

- Keeps FunC contract code separate from TypeScript wrappers
- Uses local wrappers and tests to inspect contract behavior before network interaction
- Represents code/data cells explicitly through generated TypeScript helpers
- Provides a compact example of how off-chain scripts coordinate with on-chain contracts

## Skills demonstrated

- Smart-contract project setup
- TypeScript tooling around blockchain code
- FunC contract navigation
- Test-driven contract experimentation
- Understanding proof-of-work mechanics in a modern chain environment
