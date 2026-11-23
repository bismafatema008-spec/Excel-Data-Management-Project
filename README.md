# Real Estate Plot & EMI Management Workbook

A spreadsheet prototype for organising plot-owner records, tracking installment payments, and reviewing draw-related information in one workbook.

**Project type:** Microsoft Excel / spreadsheet practice  
**Status:** Prototype — formula review required before operational use

## Workbook

[Open or download the Excel workbook](./Real%20state%20management%20project.xlsx)

The workbook contains four worksheets:

| Worksheet | Purpose |
| --- | --- |
| **Plot Owner Master** | A central table for plot numbers, owner names and contact details, plot size and rate, booking amounts, payment totals, outstanding amounts, winner status, and eligibility status. It also contains WhatsApp link/reminder fields. |
| **EMI Tracker (12 Draws)** | A repeated set of amount, date, receipt, and status fields for tracking up to 12 payment/draw entries per plot. |
| **Draw Winners (Auto)** | A table with draw number, eligible plot, eligible owner, and prize columns. |
| **Dashboard** | A summary area for total plots, collection, outstanding amount, booking collection, EMI collection, and winner count. |

## What this project is designed to practise

- Structuring records in a master worksheet
- Keeping related payment entries in a separate tracker
- Linking information across worksheets with formulas
- Presenting summary metrics in a dashboard layout
- Using spreadsheet hyperlinks for WhatsApp contact and reminder actions
- Organising a workbook around a practical real-estate administration scenario

This is a spreadsheet/data-management project, not an AI or machine-learning project.

## Open the workbook

1. Open the workbook link above and download the .xlsx file.
2. Open it in Microsoft Excel or a compatible spreadsheet application.
3. Work on a separate copy so the original project file remains unchanged.
4. Review formulas and links before entering any real information.

No additional code installation is required. Formula behaviour has not been tested across different spreadsheet applications.

## Data and privacy

The committed workbook currently uses placeholder-style records such as **Client 1**, along with sample/default values. It should be treated as a demonstration template, not as a verified customer database.

Do not add real names, phone numbers, payment details, or other personal information to a public GitHub copy. Use fictional data in any screenshots or demonstrations.

## Formula review and known limitations

A static inspection of the workbook structure found items that should be checked in Excel before anyone relies on its calculations:

1. **Dashboard references:** the dashboard formulas point to an external workbook reference, **[1]Plot Owner Master**, rather than clearly referencing the Plot Owner Master sheet in this file. Dashboard totals may therefore be stale or unavailable.
2. **Plot price formula:** cell **D2**, under the Plot Size heading, contains a formula referring to D2 multiplied by E2. This appears self-referential and may be in the wrong column; confirm the intended calculation before editing it.
3. **EMI total formula:** the Total EMI Paid roll-up should be checked against the 12 Amount columns in the EMI tracker. The current formula appears to reference a mixture of the repeated amount/date/receipt/status columns.

These are review findings, not fixes. The workbook itself has not been modified, and the calculations have not been validated by running the file in Excel or LibreOffice. Do not use it for live financial or customer records until the formulas, dashboard links, and reminder text have been reviewed and tested.

## Next improvements

- Correct and test the formula references in a separate working copy.
- Confirm the eligibility rule and draw/winner workflow.
- Add screenshots only after capturing the workbook with fictional data.
- Document a tested example showing how a booking and EMI entry flow through to the dashboard.

---

Created as a practical spreadsheet project while building foundations in data handling and software development.
