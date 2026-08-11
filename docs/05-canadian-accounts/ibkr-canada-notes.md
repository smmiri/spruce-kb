# IBKR Canada notes

Starting notes if you use Interactive Brokers Canada. Always confirm the current rules in Client Portal for **your** account — permissions change.

!!! danger "Not financial advice"
    Educational notes only.

## Working assumption

For defined-risk **credit spreads**, many Canadians begin in a **non-registered margin** account, and treat TFSA as a narrower profile until the broker confirms each strategy in writing. That matches how IBC documents TFSA options (long options, covered calls, protective puts — not a blank check for spreads). Details: [TFSA constraints](tfsa-options-constraints.md).

## Questions to ask your broker

Use this as a conversation guide when you message support or review Client Portal. It is not a form to fill on this website.

| Topic | Why it matters |
|-------|----------------|
| Options permissions for **multi-leg spreads** | Spreads need the right approval level on the account you will fund |
| CAD vs USD funding and FX conversion | Spreads on U.S. names often involve USD; conversion costs and cash balances matter |
| Margin vs cash configuration | Buying power and what strategies are allowed differ |
| Exercise and assignment notices | Short options can be assigned; you need to know how you are notified |
| Statements / Flex exports for journaling | Later you will want fills and tax lots in a reproducible export |
| Re-read [IBC TFSA/RRSP information](https://www.interactivebrokers.ca/en/accounts/rsp_tfsa_information.php) after permission changes | Published allowlists are the source of truth |

## Pattern day trader notes

U.S. PDT rules are U.S.-specific. Still respect whatever margin and account controls IBKR applies to you. Forum advice from U.S. accounts does not always map to IBKR Canada.

## Risk disclosure

Before trading options, read the OCC document *Characteristics and Risks of Standardized Options* (brokers usually require an acknowledgment). Uncovered writing risks are called out there.

## Related reading

- [TFSA options constraints](tfsa-options-constraints.md)  
- [Cash vs margin](cash-vs-margin.md)  
- [Sources](../00-meta/sources.md)  

---

*Not financial advice. Verify with IBKR Canada and advisors.*
