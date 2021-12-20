# OlyZaps

## What is OlyZaps?

OlyZaps allows users to swap (zap) any asset into sOHM or a bond directly through
the [Olympus App](https://app.olympusdao.finance/#/zap).

This is made possible through a collaboration with [Zapper](https://zapper.fi/),
which provides the back-end infrastucture for zapping.

## How do I use it?

Head over to the [OlyZaps section](https://app.olympusdao.finance/#/zap) of the
Olympus App and follow our [step-by-step guide](../using-the-website/olyzaps.md).

Note that OlyZaps for bonds is still being built out; you can only zap into sOHM
for now.

## Does OlyZaps save me gas?

OlyZaps combines a few transactions (token approval and swap) into a single transaction.
As a result, there is less exposure to gas price volatility and the gas fees you
end up paying should be the same or slightly less than performing all these
transactions separately.

## I am trying to use OlyZaps, but the quoted gas price looks expensive.

OlyZaps transaction may appear more expensive, but that is only because OlyZaps
bundles all these transactions into a single, big transaction. If you add up
the gas fees of these individual transactions, the math should work out about the
same.

As mentioned in the previous entry, OlyZaps may end up costing less because you
are not exposed to gas price volatility.
