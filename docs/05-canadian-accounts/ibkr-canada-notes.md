# IBKR Canada notes

Starting notes for Canadian retail using Interactive Brokers Canada. Confirm everything in Client Portal / in writing for **your** account.

!!! danger "Not financial advice"
    Educational notes only. Product availability and approvals change.

## Default posture

Working assumption for this curriculum: run defined-risk credit-spread process primarily in a **non-registered / margin** account until each strategy is confirmed allowed in any registered account you use.

Cross-check: IBC documents **no margin** in TFSA and lists long options / covered calls / protective puts for TFSA — not a blank check for spreads. See [TFSA constraints](tfsa-options-constraints.md).

## Confirm with the broker

- [ ] Options trading permissions / strategy approvals for **spreads** on the account you will use  
- [ ] CAD vs USD funding and FX conversion behavior  
- [ ] Margin vs cash account configuration (non-registered)  
- [ ] Exercise/assignment handling and notifications  
- [ ] Tax lot / export options (Flex queries, activity statements) for journaling  
- [ ] Re-read [IBC TFSA/RRSP information](https://www.interactivebrokers.ca/en/accounts/rsp_tfsa_information.php) after any permission change  

## Pattern day trader

US PDT rules are US-specific. Still respect **IBKR margin, pattern flags, and account configuration** that apply to you. Do not assume US forum advice maps 1:1 to IBKR Canada.

## Risk disclosure

Before trading options, read the OCC disclosure *Characteristics and Risks of Standardized Options* (brokers typically require acknowledgment). Uncovered writing risks are called out explicitly there.

## Sources

- [IBC — RRSP/TFSA/FHSA information](https://www.interactivebrokers.ca/en/accounts/rsp_tfsa_information.php)  
- [IBC — Account guide](https://www.interactivebrokers.ca/en/accounts/account-guide.php) (margin not allowed in TFSA)  
- [Sources index](../00-meta/sources.md)  

## Related

- [TFSA options constraints](tfsa-options-constraints.md)  
- [Cash vs margin](cash-vs-margin.md)  

---

*Footer: Not financial advice. Verify with IBKR Canada and advisors.*
