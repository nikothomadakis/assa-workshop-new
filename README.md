# ASSA assurance workshop

## Import and set up the workflow

Need a workshop API key? Open **[Workshop key access](access/README.md)** and use the password supplied by the facilitator.

Open **[ASSA-SINGLE-IMPORT.json](ASSA-SINGLE-IMPORT.json)**, copy the complete JSON and paste it into a new, empty n8n workflow. Alternatively download the JSON and choose **Import from File** from the workflow menu.

1. Select the same Anthropic credential in **Investigator Model**, **HAF Model** and **Report Model**.
2. Add your review framework at the top of the **HAF Agent** System Message. Keep the supplied Calculator instructions and output contract below it.
3. Save and run **Run workshop question**. Download the approved report from **HTML report file**.

All six data tools and the fixed workshop dataset are included. Framework and reference tools read public GitHub files. No Google Sheets connection or additional workflow imports are needed. **The HAF review framework is intentionally blank.**

Policy-query results identify the product and applied filters alongside their figures. The configured Anthropic model and agent nodes require a compatible n8n version and model access. Changing a Google Sheet does not change the embedded dataset. Model outputs may vary between runs.

## Canvas layout

The main path is aligned horizontally, supporting tools sit below their agents, and the setup note sits alongside the workflow. Paste into an empty workflow to avoid duplicate nodes. If the canvas opens off-centre, use **Fit to view**. Saved node coordinates control the layout; n8n controls the viewport and paste placement.

## Workshop reading and data

Open the formatted reports in your browser; no download is needed.

- **[Compare the AI and human reports side by side](https://nikothomadakis.github.io/assa-workshop-new/reports/compare.html)**
- [AI report](https://nikothomadakis.github.io/assa-workshop-new/reports/01-AI-example.html)
- [Human / HAF-approved reference report](https://nikothomadakis.github.io/assa-workshop-new/reports/02-HAF-approved-reference.html)
- [Human review framework](https://nikothomadakis.github.io/assa-workshop-new/reports/03-human-review-framework.html)
- [Workshop data and download](data/README.md)

The reports are fixed examples for the synthetic workshop case. The reference report’s approval status is illustrative.
