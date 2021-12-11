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
For this article, we added V1 and V2 after each token name to help you differentiate
between the old and new tokens. Partner websites, price aggregators, or your wallet
will not display the version information.
{% endhint %}

## What is the TLDR?

- wsOHM V1 (wrapped, staked OHM) will be replaced by gOHM (Governance OHM). They
function exactly the same, but gOHM is set up for on-chain governance.

- OHM and sOHM tokens will have their identical V2 counterparts. OHM V1 becomes
OHM V2, and sOHM V1 becomes sOHM V2.

- Token tickers will remain the same for V1 tokens. For example, after migration,
your wallet will show "OHM" instead of "OHM V1". Make sure to update the token
contract in your wallet with the [V2 addresses](../contracts/tokens.md) to show
your balances.

- When migrating OHM V1 and/or sOHM V1, you will get gOHM in return. Although
the token balance will be different (gOHM price is calculated differently, which
is based on the Current Index), the **dollar amount remains the same.**

- After the migration, OHM V1 pools such as OHM-DAI will utilize OHM V2. This applies
to new bonds as well. Partners like Abracadabra will only accept new deposits in
gOHM. So, you will need to migrate if you want to use these features. **Otherwise,
you can sit tight and migrate only when you want to.**

## What if I don't migrate?

You don't get to enjoy the new features introduced by V2. Some partners such as
Rari Capital will only accept V2 tokens once they are deployed, so you would
need to migrate if you want to spend more tokens (e.g. make new deposits) on these
platforms.

{% hint style="info" %}
Again, you would not miss any rebase rewards if you don't migrate during the migration
phase. Even if you chose to migrate way later, you will receive the same amount
of gOHM that you would have received had you migrated immediately.
{% endhint %}

## Gas fees are high now, will I lose my rebase rewards if I delay the migration?

No, you can migrate at your leisure once it goes live. The smart contract will
keep track of your entitled rebase rewards so you wouldn't miss any of them.

## What is the migration process?

When the migration is live, the Olympus front-end will be updated to allow the
migration of all your V1 tokens (i.e. OHM, sOHM, and wsOHM) to gOHM.

The migration process requires two steps: one to approve the contract for each
of your V1 tokens, and another that actually migrates all your tokens to gOHM.

{% hint style="info" %}
Each V1 token type requires its own approval step. For example, if you have OHM
V1 and sOHM V1 in your wallet, you need to perform two token approvals, but only
one migration operation (three transactions in total).
{% endhint %}

## Can I migrate a specific type of V1 token and leave out the others?

No. You can either migrate all your V1 tokens (i.e. OHM, sOHM, and wsOHM) or none
at all.

## Can I switch back to V1 tokens after migrating them to gOHM?

No, you can't switch back from gOHM to V1 tokens through our migration tool.

## Can you walk me through an example of how much gOHM I can expect from the migration?

Assuming you have 20 OHM V1, 20 sOHM V1, and 20 wsOHM, and the [Current Index](https://docs.olympusdao.finance/main/basics/basics#how-do-i-track-my-rebase-rewards)
is 10.

- 20 OHM V1 = 2 gOHM. Take your 20 OHM and divide it by the Current Index to get
your gOHM.

- 20 sOHM V1 = 2 gOHM. Take your 20 sOHM and divide it by the Current Index to
get your gOHM.

- 20 wsOHM = 20 gOHM. 1 wsOHM is equivalent to 1 gOHM.

{% hint style="info" %}
As a reminder, if you're migrating from a non-index-based token (OHM, sOHM) to an
index-based token (gOHM), you won't receive the same amount of tokens after the
migration, but they still worth the same in dollar term.
{% endhint %}

## Will my gOHM still earn rebase rewards?

Yes. Although gOHM does not change in quantity upon rebase like sOHM does, it
still earns you rebase rewards. This is because the price of gOHM is tied to the
Current Index:

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

Learn more about how bonds will behave in V2 from the [Olympus Medium page](https://olympusdao.medium.com/introducing-olympus-v2-c4ade14e9fe).

## Is Olympus V2 audited?

All V2-related contracts are live, and some of them are still under audit process.
We are working with Runtime Verification for the audit, and the results will be
published once they become available.
