## Summary
- [ ] Scope and intent are clear
- [ ] Breaking changes documented

## Type
- [ ] Site / UI change
- [ ] System / backend change
- [ ] Automation / pipeline change
- [ ] Web3 integration (contract interaction, subgraph, on-chain event)
- [ ] Infrastructure / deploy config

## Testing
- [ ] Not run (explain why)
- [ ] `npm run build` passes
- [ ] Manual testing: describe below
- [ ] Web3: tested on testnet / fork (specify)

## Web3 checklist (if applicable)
- [ ] No private keys or mnemonics in any file
- [ ] RPC URLs from env vars only
- [ ] Reentrancy / auth reviewed if touching contract calls
- [ ] Slippage/deadline params present for any swap ops

## Notes
Risks, rollbacks, flags, or follow-ups.
