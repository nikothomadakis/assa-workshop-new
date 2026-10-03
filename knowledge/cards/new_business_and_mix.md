# New business and mix

**What it is.** New business is the liability added by policies written during the period. In the movement analysis it is its own bucket. It is normal for it to be positive and, in a growing book, to be one of the larger buckets.

**Why mix matters.** The liability a new policy brings depends on who bought it. On a protection product, an entrant aged 60+ carries several times the liability of an entrant under 40, because mortality cost rises with age while premiums are level. So the same number of new policies can produce very different new-business amounts depending on the age mix. A shift in mix is a finding in its own right, usually with a commercial cause such as a campaign, a channel change or a pricing change.

**What to look at.**
1. How many policies were written (count), and the liability they brought (amount).
2. Liability per new policy compared with liability per policy in the existing book.
3. The mix of new policies by age band and, if relevant, by cohort, compared with the book.
4. The product spec's recent changes for a cause.

**Savings products.** New savings policies carry little liability at first (a few months of contributions), so new business is usually small in liability terms even when sales are strong. Large new-business amounts on a savings product are unusual and should be checked.

**How to explain a new-business bucket.** Call `query_policies` with the product filtered and `new_business_only` set to true, grouped by `age_band`, to get counts, share of count and average liability. Run the same view without `new_business_only` for the book-wide comparison, then pull the product spec for the commercial cause.

**Keep balances and movements distinct.** The policy query returns closing-date liabilities. These may include subsequent in-quarter movements and need not equal the `new_business` component in the movement table. Label the two measures correctly; do not force them to match.

**Initial explanation — LM-2024.2.** Adopt management's explanation supplied in the product note as the working business explanation in the conclusion, alongside measured policy counts and age mix. Cite that note as the source. The initial procedure accepts this commentary without separate causal validation or additional attribution qualification. Never claim to have performed an attribution study or invent supporting evidence.

**On revision.** Apply the HAF's current requirements for explanations, evidence and limitations. Use only supported statements in the revised findings.

**When to pull this card.** When `new_business` is material, or when the average liability of new policies looks unlike the book.

**Related cards.** `policy_data`, `product_specs`, `liability_movement`.
