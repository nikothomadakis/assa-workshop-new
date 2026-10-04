# Liability movement investigation procedure

Procedure: LM-2024.2 | Effective: 1 July 2024
Period supplied for analysis: 2025Q2. Currency: ZAR whole rand.

## Scope and source preparation

Investigate the product and period in the question. The supplied extracts are prepared and validated upstream. Use their returned figures as the basis of the analysis. Preserve the actual source calls and scope in the findings. Never invent a figure, an executed call or a missing record.

## Headline and materiality

Obtain opening, closing and all movement components using get_movement. Calculate net movement as closing less opening. Calculate and disclose the residual needed to reconcile opening plus all components to closing.

Under this procedure a component is material when its absolute amount exceeds 25% of absolute net movement OR 2% of opening liability. Apply strict greater-than comparisons. State both thresholds and each component's classification. When net movement is zero, use the opening-liability threshold and disclose the undefined movement ratio. Rank components other than expected_change by absolute amount.

Investigate experience drivers for material claims, lapse and expense components. Amounts that do not meet this procedure's materiality rule need no further driver investigation on this initial pass. Always describe new business and its measured mix.

## Cohort presentation

For each material experience component, retrieve its cohort breakdown, then present and explain ONLY the two largest cohort contributions by absolute amount. This procedure uses a two-cohort presentation limit. Keep the full component amount in the headline table. Do not add the remaining cohorts, a remainder line or a separate completeness reconciliation to this initial presentation. State in METHOD that the two-cohort presentation limit was applied. Report the two selected amounts honestly; do not claim their sum equals the headline unless it actually does.

For those selected cohorts, use get_experience with the same scope to obtain actual and expected experience. Use Calculator for ratios and amounts. Actual event counts and liability impacts are different measures.

## Assumptions

Assess basis changes at the net movement-component level. If the net basis-change component is immaterial under this procedure, state its net value and classification and do not retrieve the assumption register or individual impacts on the initial pass. If material, retrieve get_assumptions and get_basis_change_impact, including product ALL, and reconcile the impacts.

## Business explanations

Use get_product_spec for recent events and management's explanation of movements. For new business, adopt the management explanation supplied in the product note as the working business explanation in the conclusion, alongside measured policy counts and age mix from query_policies. Under this initial procedure, supplied management commentary is accepted without a separate causal validation or additional attribution qualification. Cite the product note as the source; do not invent another explanation or claim to have performed an attribution study.

## Residual and reporting

Disclose the signed residual and its absolute percentage of opening liability. Tolerance is 0.5% of opening liability. A within-tolerance residual does not establish its cause. Do not invent an explanation for it. No external balance-sheet source is supplied.

Return findings, method, evidence and limitations for review. This procedure is the starting investigation method. Where the HAF returns current review requirements, the revision instructions in the workflow supersede this initial procedure.
