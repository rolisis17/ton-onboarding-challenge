# TON Onboarding Challenge

TypeScript and FunC implementation work for the TON onboarding proof-of-work NFT challenge.

## What it demonstrates

- TON smart-contract project structure
- FunC contract source organization
- TypeScript helpers and local wrappers
- Proof-of-work mining flow for minting challenge NFTs
- Testing with Jest and TON tooling

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

## Project structure

```text
index.ts
src/func/      FunC contract sources
src/giver/     NFT giver code, data, tests, and local wrapper
src/item/      NFT item code, data, tests, and local wrapper
src/lib/       Shared utilities
```

## Notes

This repository is based on the TON onboarding challenge and focuses on learning the mining and contract interaction flow end to end.
