### PartyA Terminal
* `start CreateObligation longAmount: 1000, currencyCode: USD, role: OBLIGOR, counterparty: PartyB, dueBy: 1590000000, anonymous: false`
* `start NovateObligation linearId: REPLACE_W_OBLIGATION_UID, fiatIdentifier: USD, digitalIdentifier: XRP, oracle: Oracle`
### PartyB Terminal
* `start NovateObligation linearId: REPLACE_W_OBLIGATION_UID, fiatIdentifier: USD, digitalIdentifier: XRP, oracle: Oracle`
### PartyA Terminal
* `start OffLedgerSettleObligation longAmount: 20000000, digitalIdentifier: XRP, linearId: REPLACE_W_OBLIGATION_UID`