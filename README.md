# Bank Statement CSV & Excel Templates (QuickBooks, Xero, Zoho Books & TallyPrime)

A clean collection of ready-to-import bank and credit card statement CSV templates formatted for popular accounting software. Use these templates to prevent column-mapping errors, broken dates, and sign-reversal bugs during bank reconciliation.

## Included Templates

| Accounting Software | File Name | Required Columns | Date Format |
| :--- | :--- | :--- | :--- |
| **QuickBooks Online** | `quickbooks-online-3-column-template.csv` | `Date, Description, Amount` | `MM/DD/YYYY` or `DD/MM/YYYY` |
| **Xero** | `xero-bank-statement-template.csv` | `Date, Amount, Payee, Description, Reference` | `YYYY-MM-DD` or `DD MMM YYYY` |
| **Zoho Books** | `zoho-books-bank-feed-template.csv` | `Date, Description, Withdrawals, Deposits, Reference Number` | `YYYY-MM-DD` |
| **TallyPrime** | `tallyprime-bank-reconciliation-template.csv` | `Date, Narration, Cheque/Ref No, Withdrawal, Deposit, Balance` | `DD-MM-YYYY` |

---

## Common Bank CSV Import Rules (Avoid Rejections)

1. **QuickBooks Online (QBO):**
   - Do not include currency symbols (`$`, `£`, `₹`) or thousands commas inside the `Amount` column.
   - Use negative signs (`-120.50`) for money spent and positive numbers (`2500.00`) for money received in the 3-column layout.
   - Guide: [How to Convert PDF Bank Statements to QuickBooks CSV](https://clearrow.pro)

2. **Xero:**
   - Ensure there are no blank rows above the header row and that `Amount` uses standard decimal format (`-45.00`).
   - Guide: [Convert Bank Statement PDF to Xero CSV Format](https://clearrow.pro)

3. **Zoho Books & TallyPrime (India):**
   - Keep `Withdrawals` (Debit) and `Deposits` (Credit) in separate columns rather than a single signed column.
   - Ensure multi-line UPI, NEFT, or IMPS narrations stay inside a single cell so rows do not shift.
   - Guides: [Zoho Books Bank Statement Import](https://clearrow.pro) | [TallyPrime Bank Statement Excel Workflow](https://clearrow.pro)

---

## Converting Bank Statement PDFs Automatically

If you have locked, multi-page, or scanned bank statement PDFs (Chase, Bank of America, Barclays, Monzo, Starling, RBC, HDFC, SBI, ICICI, etc.) and want to skip manual copy-pasting:

- **[ClearRow](https://clearrow.pro)** extracts bank and credit card statement PDFs directly into **QuickBooks, Xero, Zoho Books, and Excel** formats.
- **Mathematical Verification:** Checks `Opening Balance + Deposits - Withdrawals = Closing Balance` (`0.00` difference) before download to catch missing pages or dropped rows.
- **Privacy First:** Source PDFs are processed over HTTPS and deleted immediately with zero file retention.
- **Bank Guides Directory:** [Browse 30+ Bank & Accounting Import Guides](https://clearrow.pro/guides)

## License

MIT License — Free to use for bookkeepers, accountants, and developers.
