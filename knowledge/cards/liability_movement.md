# Liability movement analysis

**What it is.** A liability movement analysis (also called an analysis of change or a roll-forward) explains how a liability got from its opening value at one valuation date to its closing value at the next. The total change is split into named buckets, each of which has a cause you can point to.

**The buckets used in this system.** Every bucket is a signed amount: its contribution to (closing − opening).

| Bucket | What it captures |
|---|---|
| `expected_change` | What the opening assumptions predicted would happen: discount unwind, expected claims, expected lapses, expected expenses and premiums received. This is the baseline and is not investigated further. |
| `claims_variance` | Actual claims differing from expected, converted to a liability impact. |
| `lapse_variance` | Actual lapses or surrenders differing from expected, converted to a liability impact. |
| `expense_variance` | Actual maintenance expenses differing from expected. Usually small in liability terms. |
| `basis_change` | The effect of changing assumptions during the period. Always has a paper trail in the assumptions register. |
| `new_business` | Liability added by policies written during the period. |
| `residual` | Whatever is left: closing − opening − all buckets. Never stored; always derived. |

**Why it matters.** The analysis is how an actuary checks that the liability moved for reasons they understand. A bucket that is large and unexplained is a problem; a residual that is large is a bigger one.

**How it is organised here.** The book is split into cells: product × entry-year cohort × age band. Every bucket is available per cell, so a movement can be located ("which cohort drove it?") before it is explained ("why?").

**Initial materiality — LM-2024.2.** A bucket is material when its absolute amount exceeds 25% of absolute total movement OR 2% of opening liability. Use strict greater-than comparisons and state both thresholds. If net movement is zero, use the opening-liability threshold and disclose the undefined movement ratio. The initial procedure assesses basis change on its net bucket amount; an immaterial net amount does not require register or individual-impact retrieval on that pass.

**Initial supporting analysis.** For a material experience bucket, retrieve the cohort breakdown and present only the two largest cohort contributions by absolute amount. Retain the full bucket in the headline. State the two-cohort presentation limit in METHOD; do not claim the two amounts add to the full bucket unless they do. Follow the main procedure for presentation scope.

**On revision.** The HAF's current review requirements supersede conflicting initial materiality and presentation rules. Source data remains the authority for numerical facts.

**When to pull this card.** At the start of any movement question, or when unsure what a bucket means.

**Related cards.** `experience_variance`, `basis_change`, `new_business_and_mix`, `residual_and_tolerance`.
