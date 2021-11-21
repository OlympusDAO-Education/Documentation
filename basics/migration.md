# V2 Migration

## Why do I need to migrate?

You don't have to, but we recommend you to do so. V2 migration introduces new
features such as on-chain governance and auto-staking for bonds. You can read
more about this on the [Olympus Medium page](https://olympusdao.medium.com/introducing-olympus-v2-c4ade14e9fe).

## Gas fees are high now, will I lose my rebase rewards if I delay the migration?

No, you can migrate at your leisure once it goes live. The smart contract will
keep track of your entitled rebase rewards so you wouldn't miss any of them.

## What if I don't migrate?

You don't get to enjoy the new features introduced by V2. Some partners such as
Rari Capital will only accept V2 tokens once they are deployed, so you would
need to migrate if you want to spend more tokens (e.g. make new deposits) on these
platforms.

## What is the migration process?

When the migration is live, the Olympus front-end will be updated to allow the
migration of all your v1 OHM tokens (i.e. OHM, sOHM, and wsOHM) to gOHM.

The migration process requires two steps: one to approve the contract for each
of your v1 tokens, and another that actually migrates all your tokens to gOHM.

{% hint style="info" %}
Each v1 token type requires its own approval step. For example, if you have OHM
and sOHM in your wallet, you need to perform two token approvals, but only one
migration operation.
{% endhint %}

## Can I migrate a specific type of v1 token and leave out the others?

No. You can either migrate all your v1 tokens or none at all.

## Can I switch back to v1 tokens after migrating them to gOHM?

No.

## Can you walk me through an example of how much gOHM I can expect from the migration?

Assuming you have 20 OHM, 20 sOHM, and 20 wsOHM, and the [Current Index](https://docs.olympusdao.finance/main/basics/basics#how-do-i-track-my-rebase-rewards)
is 10.

- 20 OHM = 2 gOHM. Take your 20 OHM and divide it by the Current Index to get your
gOHM.

- 20 sOHM = 2 gOHM. Take your 20 sOHM and divide it by the Current Index to get
your gOHM.

- 20 wsOHM = 20 gOHM. 1 wsOHM is equivalent to 1 gOHM.

## How are bonds affected after the migration?

In V2, you can purchase multiple bonds of the same type without resetting the
bond vesting period.

Also, there is no need to claim bond rewards and stake them manually, as this process
will be automated. The bonders will receive their entitled sOHM at the end of the
vesting period.
