# Single-import workshop workflow

Open `ASSA-SINGLE-IMPORT.json` on GitHub and copy the complete file contents into a new, empty n8n workflow. Alternatively download the JSON and choose **Import from File** from the workflow menu.

1. Select the same Anthropic credential in **Investigator Model**, **HAF Model** and **Report Model**.
2. Write your HAF review framework at the top of the **HAF Agent** System Message. Keep its supplied Calculator instructions and output contract.
3. Save, then run **Run workshop question**. Download the approved report from **HTML report file**.

All six data tools and the fixed workshop dataset are included. The framework and reference tools use public GitHub files. No Google Sheets connection or separate tool-workflow imports are required. Policy-query results identify the product and applied filters alongside their figures.

The main path is aligned horizontally, supporting tools sit below their agents, and the setup note sits next to the workflow. Paste into an empty workflow, not an existing build. If the canvas opens off-centre, use **Fit to view**. Saved node coordinates control the layout, but n8n controls the viewport and paste placement.

This is the attendee version: the HAF review framework is intentionally blank. The Calculator/output instructions remain. It includes the current tool-input and policy-scope fixes. Use only one completed workflow, not both import options.

The configured Anthropic model and agent nodes require a compatible n8n version and model access. Changing the Google Sheet does not change this fixed dataset. Model outputs may vary between runs.
