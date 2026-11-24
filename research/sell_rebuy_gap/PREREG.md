# sell-rebuy-gap-0.1 (pre-registered 2026-11-24, before any data under the new rule is scored)

Owner decision (Ali, 2026-11-24): a holder's SELL_REBUY is shown only when the gap between the price and the
buy-back support is at least 15 USD for gold (XAU) and at least 0.65 % of the price for digital assets.
Below that gap the app shows HOLD_SELL_ABOVE instead (reason: fees and spread would consume the gap).

Scope: ideas recorded from beginner-ideas-0.2 onward (ideas.py VERSION). Ideas recorded under 0.1 stay as they
are; they are not rescored and are not mixed into this evaluation.

Evaluation (fixed now):
- Population: SELL_REBUY ideas with version beginner-ideas-0.2, scored with the existing score() function.
- Compare against the same alternative already used for SELL_REBUY (holding, no sale).
- Verdict uses the existing rule: USEFUL if mean excess return after fees > 0 and the rose-without-return share
  is >= 0.5; NOT_USEFUL otherwise; INSUFFICIENT below 30 scored ideas.
- No threshold will be changed after results are seen. Any change requires a new PREREG.

Expected reading: this change is a cost filter, not a claimed edge. It is judged by whether the remaining
SELL_REBUY ideas stop losing to holding, not by how many ideas remain.
