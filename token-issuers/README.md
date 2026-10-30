# Listing a token on Tradecraft

What asset issuers need to list a CIP-56 token on Tradecraft and seed its first pool.

Tradecraft is the largest decentralized exchange on Canton by total value locked and asset volume. Tradecraft does not issue tokens; it lists them. The issuer brings the token and liquidity, and Tradecraft brings the market makers, inventory providers, and trading volume that turn a pool into a market.

This page covers the requirements and the process for a listing.

## How a listing works <a href="#how-it-works" id="how-it-works"></a>

A listing on Tradecraft is a liquidity pool pairing the issuer’s token with Canton Coin (CC), seeded to a minimum depth and traded against by Tradecraft’s inventory-provision bot and partner market makers. That trading activity creates validated volume on Canton for the token.

| Participant         | What they bring                                                                                         | What they get                                          |
| ------------------- | ------------------------------------------------------------------------------------------------------- | ------------------------------------------------------ |
| Issuer              | A live CIP-56 token, a price feed, and the initial liquidity (its own or from its liquidity providers). | A liquid market for the token on Canton’s largest DEX. |
| Tradecraft          | Pool creation, the inventory-provision bot, and market-maker relationships.                             | Trading volume and depth on the venue.                 |
| Liquidity providers | Pairs of tokens deposited into the pool so trades have inventory to settle against.                     | Swap fees in proportion to their share of the pool.    |

## Requirements <a href="#requirements" id="requirements"></a>

Each of these is confirmed on the introductory call. Several can be in progress at the start.

| Requirement         | Details                                                                                                                                                                                                             |
| ------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Live CIP-56 token   | The token is live on Canton mainnet as a CIP-56 asset, or within a few weeks of launch. The pool can be created ahead of launch so trading opens on day one.                                                        |
| Reliable price feed | A centralized reference price: an API, or a listing on an exchange that is not another DEX. Tradecraft’s bot prices the pool against it.                                                                            |
| Security audit      | Market makers and third-party liquidity providers do not deploy capital without a completed audit verifying the token’s backing. For bridged tokens, documentation of the bridge’s security model is also required. |
| Minimum liquidity   | $150,000 total value locked in the first pool, split evenly: $75,000 of the token and $75,000 of CC. Liquidity can come from the issuer, the issuer’s liquidity providers, or both.                                 |
| Token icon          | A square icon for the token, used in the Tradecraft interface and by integrated wallets.                                                                                                                            |

**There is no listing fee.** The only capital requirement is the liquidity in the pool, which remains in the control of whoever deposited it.

## The listing process <a href="#process" id="process"></a>

Every listing follows the same six steps. Pool creation takes one to two days once Tradecraft has the token and icon; the overall timeline is usually set by how quickly liquidity is ready.

1.  ### Introductory call

    Both teams

    Tradecraft and the issuer walk through the token, the timeline, and the terms on this page. The issuer should be ready to cover:

    * Whether the token is live on Canton
    * The price-feed source
    * Current and upcoming exchange listings
    * Audit status, and bridge security documentation if the token is bridged
2.  ### Agree terms and sign

    Both teams

    Both sides agree on the commercial terms and the liquidity commitment, and sign the agreement.
3.  ### Shared Slack channel

    Tradecraft

    Tradecraft opens a channel with the stakeholders from both teams. Everything from this point happens there: receiving addresses, test results, and announcement timing.
4.  ### Pool creation

    IssuerTradecraft

    The issuer sends roughly $10 worth of the token and the token icon to the address shared in Slack. Tradecraft’s engineering team creates the TOKEN/CC pool and its pool address and runs a test transaction against it. This takes one to two days.
5.  ### Seed the pool

    Issuer

    The issuer or its liquidity providers deposit the initial liquidity. Once the $150,000 minimum is met, Tradecraft runs a swap test and opens the pool publicly.
6.  ### Go live

    Both teams

    Tradecraft and the issuer coordinate the public announcement, and Tradecraft’s inventory-provision bot and partner market makers begin trading the pool.

## Issuer rewards <a href="#economics" id="economics"></a>

Depending on an issuer’s status on the Canton network, issuers can earn Canton issuer rewards on the volume generated on Tradecraft, in a compliant manner. Tradecraft covers the specifics on the introductory call.

## Pairing and liquidity guidelines <a href="#guidelines" id="guidelines"></a>

* **The first pair is against CC.** The first pool pairs the token with Canton Coin.
* **Additional pairs use other approved assets.** After the CC pool, further pairs can be added against other assets approved for CIP-56 pairs. Not every asset is approved yet, so pairs should be confirmed with Tradecraft before being planned around.
* **Pools should stay above $100,000.** Market makers need depth to stay competitive. If liquidity drops below this level, volume falls with it.

## Inventory-providing assistance <a href="#inventory" id="inventory"></a>

Tradecraft can provide issuers with inventory-providing assistance: Tradecraft runs its inventory-provision app on the issuer’s behalf using the issuer’s own inventory. Setup and terms are covered on the introductory call.

## Meeting the liquidity minimum <a href="#lps" id="lps"></a>

Issuers that need help meeting the listing minimum can ask Tradecraft for introductions to liquidity providers it works with. Participation is not guaranteed: providers decide independently, and they will want to see the token’s audit first. See [How to Provide Liquidity](https://docs.tradecraft.fi/using-tradecraft/guide-how-to-provide-liquidity) for how deposits work.

## Frequently asked <a href="#faq" id="faq"></a>

### How long does a listing take?

Pool creation takes one to two days once Tradecraft has the token and icon. Overall timing is usually set by when liquidity is ready.

### Does Tradecraft issue or custody the token?

No. Tradecraft lists the token and brings trading activity to it. The token remains the issuer’s, and liquidity in the pool remains withdrawable by whoever deposited it.

### Can an issuer list more than one token?

Yes. Each token gets its own CC pool with its own minimum liquidity.

## Changes and updates <a href="#changes" id="changes"></a>

The requirements and terms on this page reflect how Tradecraft onboards issuers as of October 2026. Canton network rules change, and when a change affects listings, Tradecraft updates this page.

## Get started <a href="#get-started" id="get-started"></a>

Prospective issuers can email [partnerships@tradecraft.fi](mailto:partnerships@tradecraft.fi) with the following to schedule an introductory call:

* Token name and ticker, and whether it is live on Canton
* Price-feed source
* Current or upcoming exchange listings
* Audit status, plus bridge security documentation if the token is bridged
* Expected liquidity and target listing date

[Email the partnerships team](mailto:partnerships@tradecraft.fi?subject=Listing%20a%20token%20on%20Tradecraft)
