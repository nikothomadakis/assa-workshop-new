# Basis change

**What it is.** A basis change is the effect on the liability of changing the assumptions used to value it. The same policies, valued on new assumptions, produce a different number; that difference is the basis change.

**It always has a paper trail.** Assumption changes are approved and recorded in the assumptions register with an old value, a new value and a rationale. A basis change in the movement analysis without a matching register entry is itself a finding, and so is a register entry with no impact.

**The register holds this period only.** Every entry in the register belongs to the quarter under analysis, so there is no date test to apply: each change contributes to this period's `basis_change`. In a system covering several periods you would filter by effective date, and a change effective before the period would already sit in the opening liability.

**One total, several steps.** `movement.basis_change` is the total per cell. `basis_change_detail` splits it by assumption, applied as numbered steps in a fixed order. Individual step impacts depend on the order in which the changes were run; the total does not. Individual impacts can have different signs. Under LM-2024.2, the initial investigation uses the net movement-component amount to decide whether further basis work is required.

**Typical directions.** Raising expense inflation increases the liability (more future expenses to provide for). A mortality improvement on a protection product reduces the liability (fewer expected claims). Lowering a discount rate increases the liability.

**How to investigate.** On the initial pass, compare the absolute net basis-change bucket with the main procedure's 25% of absolute net movement OR 2% of opening thresholds. If it is immaterial, report the net amount and classification without retrieving the register or individual impacts. If it is material, call `get_assumptions`, including product `ALL`, and `get_basis_change_impact` with `assumption_id` blank. Report the retrieved impacts and reconcile their sum to the bucket. If a net total is zero, do not calculate shares of that net total.

**On revision.** Follow the HAF's current requirements, including any request to retrieve the complete register and individual impacts. The initial net-only selection rule does not restrict a revision.

**When to use this card.** When the initial net basis-change bucket is material, when a definition is needed, or when the HAF requests further basis-change work.

**Related cards.** `liability_movement`, `residual_and_tolerance`.
