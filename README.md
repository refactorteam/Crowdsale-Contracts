![](https://github.com/refactorteam/Crowdsale-Contracts/blob/master/images/refactor_logo.jpg)

# ReFactor Crowdsale Contracts

Ethereum smart contracts that distribute re:factor tokens (REFT).

# re:factor Token (REFT)

REFT is an ERC-20 compatible token.

1.	The token contract is created by the crowdsale contract;
2.	REFT has fixed total supply;
3.	Tokens offered for the crowdsale are transferred to the crowdsale contract at creation time;
4.	5,000,000 REFT are reserved for pre-sale investors;
5.	All remaining tokens are stored on re:factor balance.

REFT movement is restricted until explicitly allowed. Only parties authorized to transfer REFT until that are:
1.	The crowdsale contract -- to distribute tokens purchased at the crowdsale;
2.	re:factor -- to distribute among the team and pre-sale investors.

# Pre-Sale Contract
5,000,000 of tokens has been distributed during the pre-sale phase. Pre-Sale starts at the specified timestamp and ends when either the specified timestamp is reached or all the tokens are sold.

# Crowdsale Contract
The amount of tokens offered for the crowdsale is transferred to the crowdsale contract at the instantiation time. The crowdsale starts at the specified timestamp and ends when either the specified timestamp is reached or all the tokens are sold. In the former case undistributed tokens are transferred back to re:factor.

# Pricing
The tokens are sold in tranches, each tranche comprising a fixed amount of tokens at a fixed price. After all the tokens in a tranche are sold out, the next tranche becomes active.

# KYC
Only registered investors are allowed to take part in the crowdsale.

# Refund
No change as tokens are sold in token subunits and the price of a subunit is infinitesimal. If some investor hits the hard cap, her change will be refunded with a manual Ether transfer.

# Finalization
If the crowdsale ends, but not all the tokens offered are sold out, all remaining tokens are transferred to re:factor.

<a target="_blank" href="http://refactor.pro">ReFactor</a>
