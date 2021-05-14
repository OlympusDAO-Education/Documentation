# FAQs

### Why do we need OlympusDAO in the first place?

Dollar-pegged stablecoins have become an essential part of crypto due to their lack of volatility as compared to tokens such as Bitcoin and Ether. Users are comfortable with transacting using stablecoins knowing that they hold the same amount of purchasing power today vs. tomorrow. But this is a fallacy. The dollar is controlled by the US government and the Federal Reserve. This means a depreciation of dollar also means a depreciation of these stablecoins.

OlympusDAO aims to solve this by creating a non-pegged stablecoin called OHM. By focusing on supply growth rather than price appreciation, OlympusDAO hopes that OHM can function as a currency that is able to hold its purchasing power regardless of market volatility.

### OHM is backed, not pegged.

Each OHM is backed by 1 DAI, not pegged to it. Because the treasury backs every OHM with at least 1 DAI, the protocol would buy back and burn OHM when it trades below 1 DAI. This has the effect of pushing OHM price back up to 1 DAI. OHM could always trade above 1 DAI because there is no upper limit imposed by the protocol. Think pegged == 1, while backed >= 1.

You might say that the OHM floor price or intrinsic value is 1 DAI. We believe that the actual price will always be 1 DAI + premium, but in the end that is up to the market to decide.

### How does it work?

At a high level, OlympusDAO consists of its protocol managed treasury, protocol owned liquidity, bond mechanism, and high staking rewards that are designed to control supply expansion.

Bond generates profit for the protocol, and the treasury uses the profit to mint OHM and distribute them to stakers. With LP bond, the protocol is able to accumulate liquidity to ensure the system stability.

### What is the deal with (3,3) and (1,1)?

(3,3) is the idea that, if everyone cooperated in Olympus, it would generate the greatest gain for everyone (from a [game theory](https://en.wikipedia.org/wiki/Game_theory) standpoint). Currently, there are three actions a user can take:

- Staking (+3)
- Bonding (+1)
- Selling (-3)

Given two actors, all scenarios of what they could do are shown here:

![](../.gitbook/assets/faqs/game_theory.png)

If we both stake (3, 3), it is the best thing for both of us and the protocol (3 + 3 = 6).<br>
If one of us stakes and the other one bonds, it is also great because staking takes OHM off the market and put it into the protocol, while bonding provides liquidity and DAI for the treasury (3 + 1 = 4).<br>
When one of us sells, it diminishes effort of the other one who stakes or bonds (1 - 1 = 0).<br>
When we both sell, it creates the worst outcome for both of us and the protocol (-3 - 3 = -6).

### Why is PCV important?

As the protocol controls the funds in its treasury, OHM can only be minted or burned by the protocol. This also guarantees that the protocol can always back 1 OHM with 1 DAI. You can easily define the risk of your investment because you can be confident that the protocol will indefinitely buy OHM below 1 DAI with the treasury assets until no one is left to sell. You can't trust the FED but you can trust the code.

As the protocol accumulates more PCV, more runway is guaranteed for the stakers. This means the stakers can be confident that the current staking APY can be sustained for a longer term because more funds are available in the treasury. 

### Is this a Ponzi scheme?

[This Investopedia page](https://www.investopedia.com/terms/p/ponzischeme.asp) defines a Ponzi scheme as a fraudulent investing scam promising high rates of return with little risk to investors. This is similar to a pyramid scheme in that both are based on using new investors' funds to pay the earlier backers. Both Ponzi schemes and pyramid schemes eventually bottom out when the flood of new investors dries up and there isn't enough money to go around. At that point, the schemes unravel.

First, OlympusDAO is not fraudulent. The smart contracts that power OlympusDAO are public and can be verified by anyone. The treasury balances are updated in real-time and can be verified in any Ethereum block explorer such as [Etherscan](https://etherscan.io/address/0x886ce997aa9ee4f8c2282e182ab72a705762399d). This ensures transparency and allows the investors to vet the project before making an investment decision.

Second, all speculative financial instruments can only generate holder returns in one of two ways: 1) Grow its net asset value (NAV); 2) Achieve price appreciation such that later investors will buy from early investors at a premium. If you think a company or a token is only worth the amount of cash it has, then Tesla is a Ponzi, as its market cap-to-cash ratio is a whopping 37:1 (as of Q1 2021) and does not generate a penny of dividend to shareholders. The Bitcoin protocol has a market cap-to-cash ratio of infinity as it does not hold a single USD, nor does it generate income not denominated in bitcoin.

Third, OlympusDAO is not a piggy bank whose sole source of income is new infusions of cash. In fact, OHM has a compelling value proposition - it aims to become a crypto stable currency that is backed by real crypto assets in its own treasury (DAI, LP token, etc. as decided by the DAO). Currently, OHM has an intrinsic floor of 1 DAI per 1 OHM, but that's not its market price just as Tesla is worth more than the amount of cash it holds.

Lastly, in OHM's growth and expansion phase, the premium of market value over its intrinsic value will be high as the Protocol builds up its treasury. The buyers are likely to price in the NAV and a premium of future dividend expectations. In OHM's mature and stability phase, the Protocol will convert OHM price volatility to supply volatility. This is achieved by conducting open market operations from its treasury to maintain the price of OHM at a market equilibrium price. The premium of OHM will then necessarily shrink. However, OHM stakers will be protected as their balance will rebase accordingly to maintain their purchasing power. So, unlike a Ponzi scheme where profits only come from the late entrants, the Protocol actually employs strategies to preserve an investor's capital.
