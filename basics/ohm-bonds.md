Per OIP-114, OlympusDAO has launched two OHM Bond markets!

These bonds are available through the Olympus dApp: https://app.olympusdao.finance/#/bonds
 
To learn more about how we are rolling out OHM bond markets, read [this.] (https://ohm.fyi/lw1)

Alternatively users can find these bonds on the [Bond Protocol dApp.] (https://app.bondprotocol.finance) 

If you need guidance on using Bond Protocol, check out the [docs.] (https://docs.bondprotocol.finance/bond-marketplace/purchasing-a-bond)

We have included a chart to help you compare OHM Bond discounts in relation to existing staking rates. For more detailed information, make a copy of [this Google Sheet] (https://ohm.fyi/8fr)

NOTE: If you can’t secure a bond, do not worry. You’ll have a second opportunity next week, October 12th, through the Gnosis Auction. We’ll share more information next week.

[Staking rate vs. OHM helper](../../.gitbook/assets/staking-rate-vs-ohm-helper.png)

## Context
Per OIP-114 (Tantalus), Olympus will be conducting a trial run of OHM bonds. The goal will be to understand the market demand for OHM bonds and analyze the relationship between discount rate and bond maturity by utilizing two different maturity lengths. This testing and analysis will be important data to inform the development of the bond markets and the transition to a bond-centric Olympus protocol.

## Setup
Setup
We will be utilizing two auction mechanisms for price discovery: Sequential Dutch Auction (also known as Olympus-style Bond Auction) and Gnosis Auction. You can learn more about each mechanism in Bond Protocol Guide and Gnosis Auction Guide.

Each auction will launch with two bond markets: 1) fixed-maturity dated 14-day after market launch, and 2) fixed-maturity dated 28-day after market launch. Users will be able to bond OHM and receive an ERC-20 bond token. At maturity, the bond token can be redeemed for OHM. Capacity for each bond market will be 10,000 OHM. 

The launch timeline is as follows:
On Wed, October 5th: launch 2 Sequential Dutch Auction markets on Bond Protocol, one with October 19th, 2022 maturity, and another with November 2nd, 2022 maturity.
On Wed, October 12th: launch 2 Gnosis Auction markets, one with November 2nd, 2022 maturity and another with November 16th, 2022 maturity. The reason for a 7-day added lag is because of how Gnosis Auctions determine clearing price.

[Auction details](../../.gitbook/assets/ohm-bond-auction.png)

Keep in mind that Gnosis Auction requires a total minimum interest of 1,000 OHM to close successfully, otherwise all funds will be distributed back. 

## How can I participate?
We will run Sequential Dutch Auction bond markets through the Bond Protocol website, available at https://app.bondprotocol.finance. The first bond market launches October 5th. 

We will run Gnosis Auction bond markets through the Gnosis website, available at https://gnosis-auction.eth.link/#/overview#topAnchor. The first bond market launches October 12th.

Unsure about which auction to participate in? Here are some considerations for you to make an informed decision:
Price discovery - Sequential Dutch Auction locks the price at your chosen market discount. Gnosis Auction runs for 7 days and calculates a final clearing price based on all bids in that timeframe. 
Canceling orders - With Gnosis Auction, you can cancel your limit order right up to the auction close. With Sequential Dutch Auction, you secure a bond at the time of purchase.

## Participating via Bond Protocol UI
### Bidding Token: OHM token (0x64aa3364F17a4D01c6f1751Fd97C2BD3D7e7f1D5)
### Auction Token: (available once deployed)
####Instructions: 
Navigate to https://app.bondprotocol.finance/ and follow instructions Bond Protocol Auction Guide
Earliest available participation date: October 5th

## Participating via Gnosis UI
### Bidding Token: OHM token (0x64aa3364F17a4D01c6f1751Fd97C2BD3D7e7f1D5)
### Auction Token: (available once deployed)
#### Instructions: 
Navigate to LINK and follow instructions Gnosis Auction Guide
At conclusion of auction (7 days), a clearing price will be determined and, if you win, you will receive Auction Token.
Earliest available participation date: October 12th
