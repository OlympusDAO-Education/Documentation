## Bonding
Olympus bonds are a financial primitive for protocols to acquire assets, including their own liquidity, in exchange for governance tokens at a discount. In other words, Olympus bonds are a pricing mechanism for any two ERC-20 tokens that does not rely on third parties like oracles. Olympus bonds internally respond to supply and demand by offering a variable ROI rate to the market and its users. 

# How do both the Olympus Treasury and the bonder benefit from the process?
Bonds are the primary mechanism for Treasury inflows, and thus, the growth of the network.

Bonders commit a capital sum upfront and are promised a fixed return at a set point in time; that return is in OHM and thus the bonder's profit would depend on OHM price when the bond matures. In Olympus v2, users who bond their assets for OHM reap the same benefits as stakers as OHM is automatically staked at the time of a bond purchase. 

If the ROI is positive – a bond can be purchased at a discount to market price) – market participants (bonders) are incentivized to exchange their assets for gOHM, vested over a period of time. The Treasury sells OHM at a premium to its backing, while the bonder is able to capture a discount (positive ROI) by purchasing OHM directly from the Treasury. However, if the variable ROI is negative, and market participants are unable to express their demand on the bond marketplace, they would have to resort to a decentralized exchange. 

The variable ROI rate is at the one hand determined by the demand for the given bond on the Olympus bond marketplace, and on the other hand it is governed by the policy team which sets the BCV which determines the bond capacity. In exchange for being temporarily illiquid, and exposed to OHM/gOHM volatility for the duration of the vesting period, the bonder is rewarded with a variable ROI rate. 

Per OIP-114, OlympusDAO has launched two OHM Bond markets!

These bonds are available through the Olympus dApp: https://app.olympusdao.finance/#/bonds 


To learn more about how we are rolling out OHM bond markets, read this: LINK

Alternatively users can find these bonds on the Bond Protocol dApp: https://app.bondprotocol.finance 

If you need guidance on using Bond Protocol, check out: https://docs.bondprotocol.finance/bond-marketplace/purchasing-a-bond

We have included a chart to help you compare OHM Bond discounts in relation to existing staking rates. For more detailed information, make a copy of this Google Sheet https://docs.google.com/spreadsheets/d/1MccMLFXMburkiRvoC59R9KgmEPW9_OFxqg2d5n9vme8/edit?usp=sharing

NOTE: If you can’t secure a bond, do not worry. You’ll have a second opportunity next week, October 12th, through the Gnosis Auction. We’ll share more information next week.

Updated Graphic 


Context
Per OIP-114 (Tantalus), Olympus will be conducting a trial run of OHM bonds. The goal will be to understand the market demand for OHM bonds and analyze the relationship between discount rate and bond maturity by utilizing two different maturity lengths. This testing and analysis will be important data to inform the development of the bond markets and the transition to a bond-centric Olympus protocol.
Setup
We will be utilizing two auction mechanisms for price discovery: Sequential Dutch Auction (also known as Olympus-style Bond Auction) and Gnosis Auction. You can learn more about each mechanism in Bond Protocol Guide and Gnosis Auction Guide.

Each auction will launch with two bond markets: 1) fixed-maturity dated 14-day after market launch, and 2) fixed-maturity dated 28-day after market launch. Users will be able to bond OHM and receive an ERC-20 bond token. At maturity, the bond token can be redeemed for OHM. Capacity for each bond market will be 10,000 OHM. 

The launch timeline is as follows:
On Wed, October 5th: launch 2 Sequential Dutch Auction markets on Bond Protocol, one with October 19th, 2022 maturity, and another with November 2nd, 2022 maturity.
On Wed, October 12th: launch 2 Gnosis Auction markets, one with November 2nd, 2022 maturity and another with November 16th, 2022 maturity. The reason for a 7-day added lag is because of how Gnosis Auctions determine clearing price.

Auction
Launch Date
Bond Market
Capacity
Minimum
Sequential Dutch Auction
Oct 5th
Oct 19, 2022 maturity (+ 14 days)
10,000 OHM
1 OHM
Sequential Dutch Auction
Oct 5th
Nov 2, 2022 maturity (+ 28 days)
10,000 OHM
1 OHM
Gnosis Auction
Oct 12th
Nov 2, 2022 maturity (+ 14 days + 7 days)
10,000 OHM
1 OHM
Gnosis Auction
Oct 12th
Nov 16, 2022 maturity (+ 28 days + 7 days)
10,000 OHM
1 OHM


Keep in mind that Gnosis Auction requires a total minimum interest of 1,000 OHM to close successfully, otherwise all funds will be distributed back. 

How can I participate?
We will run Sequential Dutch Auction bond markets through the Bond Protocol website, available at https://app.bondprotocol.finance. The first bond market launches October 5th. 

We will run Gnosis Auction bond markets through the Gnosis website, available at https://gnosis-auction.eth.link/#/overview#topAnchor. The first bond market launches October 12th.

Unsure about which auction to participate in? Here are some considerations for you to make an informed decision:
Price discovery - Sequential Dutch Auction locks the price at your chosen market discount. Gnosis Auction runs for 7 days and calculates a final clearing price based on all bids in that timeframe. 
Canceling orders - With Gnosis Auction, you can cancel your limit order right up to the auction close. With Sequential Dutch Auction, you secure a bond at the time of purchase.

Participating via Bond Protocol UI
Bidding Token: OHM token (0x64aa3364F17a4D01c6f1751Fd97C2BD3D7e7f1D5)
Auction Token: (available once deployed)
Instructions: Navigate to https://app.bondprotocol.finance/ and follow instructions Bond Protocol Auction Guide
Earliest available participation date: October 5th

Participating via Gnosis UI
Bidding Token: OHM token (0x64aa3364F17a4D01c6f1751Fd97C2BD3D7e7f1D5)
Auction Token: (available once deployed)
Instructions: 
Navigate to LINK and follow instructions Gnosis Auction Guide
At conclusion of auction (7 days), a clearing price will be determined and, if you win, you will receive Auction Token.
Earliest available participation date: October 12th
