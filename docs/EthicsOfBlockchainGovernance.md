# Ethics of Blockchain Governance

## Principles

1. One `de facto` governs some thing if one can create and destroy that thing.
1. Governance by voting is always `de jure` if the voting system is unable to enforce (automatically) the implementation of the tally's outcome.
2. Governance by voting has 2 main types:
  - ephemeral, timebound voting: for decisions with finality (such is the governance on chains like Cosmos at this moment)
  - eternal, continuous voting: for decisions that may change, but a temporary decision has to be accounted now (this was implemented in The Laurel Project)
4. The governance `de jure` must faithfully resemble the governance `de facto`.
1. A blockchain is created by developers. By principle (1), they have the `de facto` governance in full until they cede it (or part of it), (by consensus), to the validators.
1. The governance state must be independently stored from the governed state (the rest of the chain). In case there must be layered governance, each layer should have its own chain. This way a superior layer of governance may fully reset (re-instate the genesis of) an inferior layer without losing its own state. Governance coin (voting weight) and gas should also be layer-unique.
1. The value-carrying coin (usually the coin of the main chain) begins to carry a value only after an exchange with other value-carrying coins is ratified (tested and (by consensus) announced).
1. The chain creators (developers) have to test the chain bridges using testchains of other chains (without a coin value), as well as advertised compatibility before the native coin is free to carry value. At the end of testing, they have to reach a consensus that proof of chain continuity (a state-preserving upgrade)`in vivo` has been produced.
1. After the developers obtain chain continuity, they cede part of governance to validators and will guide the validators to obtain chain continuity with their own means, and reach their own consensus on that fact.
1. Access to exchanges should be announced after chain continuity is proven by validators and a significant airdrop/claim percentage is reached (or after the claim period). This way the trade is not influenced significantly by the claim ramp-up.


## Governance Layers

- users govern (by gas vote):
  - state of contracts
- validators (by proof of stake):
  - state continuity
  - block creation
  - value of chain tokens
- blockchain developers (by proof of knowledge and goodwill):
  - sourcecode of the chain
  - deployments
  - testing (including from the point of view of validators and users)
  - releasing of governance to the validators
- blockchain founders/CEO (by proof of successful (previous) governance):
  - hiring developers
  - governing strategy

There are 3 main layers of governance: by stake, knowledge & goodwill, and previous governance.

## Conclusions

1. `de facto` governance examples:
    1. git commands that mutate the repo head
    2. PoS block validation
    3. outcome of execution of chain transactions (vote with the wallet by transaction sender)
3. `de jure` governance examples:
    1. Cosmos-type governance (even when the results are on-chain, the outcome cannot be automatically-enforced nor on-chain verified)
    2. polls among the decision-makers on Discord, etc.
5. Blockchain developers must become validators before they can cede that attribute to other players. It is their responsibility to create, instantiate, and test the validation and upgrade/migration while the coin and gas have no value (before the public phase of a launch).
6. At least one validator must be (or represent) the dev team at all times - for ease of debugging.
7. If devs have to listen to lawyers when they vote in on decisions, the lawyers have to present their moral or legal case based on clearly understandable principles, not on fear of the unknown.
