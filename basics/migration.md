# V2 Migration

## Why do I need to migrate?

V2 migration introduces new features such as on-chain governance and auto-staking
for bonds.

Transitioning from sOHM V1 to gOHM allows for multiple bonds to be taken at one
time, as opposed to one bond per vesting period as it was in v1.

Partial liquidity will remain for v1 OHM while the migration is in progress. This
provides sufficient liquidity for borrowers to close or move their borrowing
position.

You can read more about this on the [Olympus Medium page](https://olympusdao.medium.com/introducing-olympus-v2-c4ade14e9fe).

{% hint style="info" %}
You have **two months to migrate after V2 launch.** If you don't, your sOHM V1
balance will stop rebasing, but the difference will be honored when you migrate.
{% endhint %}

{% hint style="info" %}
For this article, we added V1 and V2 after each token name to help you differentiate
between the old and new tokens. Partner wbsites, price aggregators, or your wallet
will not display the version information.
{% endhint %}

## What is the TLDR?

- The wrapped sOHM token (wsOHM) will be replaced by Governance OHM (gOHM). They
function exactly the same, but gOHM is set up for on-chain governance.

- OHM and sOHM tokens will have their identical v2 counterparts. OHM becomes v2
OHM, and sOHM becomes v2 sOHM.

- gOHM will roll out first ahead of v2 OHM and v2 sOHM.

- When migrating v1 OHM and/or v1 sOHM, you will get gOHM in return. Although
the token balance will be different (gOHM price is calculated differently, which
is based on the Current Index), the **dollar amount remains the same.**

- After the migration, OHM pools such as OHM-DAI will utilize v2 OHM. This applies
to new bonds as well. Partners like Abracadabra will only accept new deposits in
gOHM. So, you will need to migrate if you want to use these features. Otherwise,
you can sit tight and migrate only when you want to.

{% hint style="info" %}
You have **two months to migrate.** If you don't, your sOHM balance will stop
rebasing, but the difference will be honored when you migrate.
{% endhint %}

## What if I don't migrate?

You don't get to enjoy the new features introduced by V2. Some partners such as
Rari Capital will only accept V2 tokens once they are deployed, so you would
need to migrate if you want to spend more tokens (e.g. make new deposits) on these
platforms.

## Gas fees are high now, will I lose my rebase rewards if I delay the migration?

No, you can migrate at your leisure once it goes live. The smart contract will
keep track of your entitled rebase rewards so you wouldn't miss any of them.

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

## Will my gOHM still earn rebase rewards?

Yes. Although gOHM does not rebase like sOHM does, it still earns you rebase rewards.
This is because the price of gOHM is tied to the Current Index:

$$
gOHM_{price} = OHM_{price} * CurrentIndex
$$

Every rebase event will cause the Current Index to go up, and your gOHM is worth
more as a result (provided that OHM's price stays constant).

## How are bonds affected after the migration?

In V2, you can purchase multiple bonds of the same type without resetting the
bond vesting period.

Also, there is no need to claim bond rewards and stake them manually, as this process
will be automated. The bonders will receive their entitled sOHM at the end of the
vesting period.
