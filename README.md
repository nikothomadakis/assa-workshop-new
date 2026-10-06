# ASSA assurance workshop

## Start with the single-import workflow

Open **[ASSA-SINGLE-IMPORT.json](ASSA-SINGLE-IMPORT.json)**, copy the complete JSON and paste it into a new, empty n8n workflow. You can also download the file and use **Import from File**.

- Select your Anthropic credential in the three model nodes.
- Add your review framework at the top of the HAF Agent System Message. Keep the supplied Calculator instructions and output contract below it.
- Save and run the workshop question.

All six data tools and the fixed workshop data are included. Framework and reference tools read public GitHub files. No Google Sheets connection or additional workflow imports are needed. **The HAF review framework is intentionally blank.**

Read [the setup and layout notes](SINGLE-IMPORT.md). If the canvas opens off-centre, use **Fit to view**. Paste into an empty workflow to avoid duplicate nodes.

## Workshop reading

- [Compare the AI and human reference reports](https://nikothomadakis.github.io/assa-workshop-new/reports/compare.html)
- [Human review framework](https://nikothomadakis.github.io/assa-workshop-new/reports/03-human-review-framework.html)
- [Workshop data](data/README.md)

## Existing pre-work build

[COMPLETE-TARGET-REFERENCE.json](COMPLETE-TARGET-REFERENCE.json) is the alternative for attendees who already configured the separate Google Sheets tool workflows. It also leaves the HAF review framework blank. Choose one workflow version; do not import both into the same canvas.
