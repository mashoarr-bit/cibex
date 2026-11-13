# CIBEX

**A free, offline reader for Bangladesh Bank CIB reports, built for the risk management community of banks and financial institutions in Bangladesh.**

Drop a CIB report PDF into CIBEX and, within seconds, it reads every contract and every month of history and lays the facts out clearly: what is classified now, where and when payments were late, which facilities were rescheduled, how limits are being used, and much more.

CIBEX was first built for my own personal use as a credit risk professional. It is now released, free, for everyone who does this work.

![CIBEX Assessment tab](docs/screenshots/1_assessment.png)

---

## Download and use

1. Download **[CIBEX_v1.0.html](CIBEX_v1.0.html)** (click the file, then the download button).
2. Open it in **Google Chrome** or **Microsoft Edge**.
3. Drop one or more CIB report PDFs onto the page, or click to choose them.

There is nothing to install, no account and no login. The file works with the internet switched off.

---

## Your data never leaves your computer

* CIBEX is a single HTML file that runs entirely in your browser.
* It does not upload anything and does not connect to any server. Everything it needs, including the PDF reader and the chart library, is inside the file.
* Reports you open are kept only until you close the browser tab.
* There is no tracking and no analytics of any kind.

You can check this yourself: disconnect from the internet and CIBEX still works.

---

## What CIBEX shows

| Tab | What you get |
|---|---|
| **Assessment** | Facilities classified now (as borrower and as guarantor), late payment by year, and plain checks answered Yes or No with the contract codes behind each one. |
| **Contracts** | Every facility in one table with a 24 month repayment strip, and the full monthly history of each contract. |
| **Analytics** | How long ago the last overdue, 30+, 90+ and classified month was; the trend in use of overdraft, cash credit and card limits over 24 months; and a DBR calculator. |
| **Summary** | Subject details, totals by role and classification, and the reporting institutions. |
| **Data Checks** | Points in the report that need a second look, such as figures that do not agree, and how completely the report was read. |

### Checks in the Assessment tab

For the borrower and co borrower, and separately for the guarantor, CIBEX answers Yes or No for each of these and lists the contracts behind every Yes:

* overdue now; X DPD, 30+, 60+ and 90+ DPD in the last 12 months; 90+ DPD at any time
* repayment getting worse over time
* Special Mention (SMA) in the last 12 months; classified in the past; classified now
* marked as default or wilful default
* rescheduled at any time or in the last 12 months; reorganised credit
* law suit filed; stay order
* limit use above 95%; outstanding above the sanctioned limit now
* contract end date passed but the facility is still living
* new facility in the last 6 or 12 months
* remarks recorded by the lender; facility with the bank that requested the report

All counting is anchored to the inquiry date of the report.

### DBR calculator

Enter the net monthly income and the proposed EMI. CIBEX adds the EMI of the living borrower and co borrower term loans from the CIB, a share of the credit card limits, and a monthly amount for overdraft, cash credit, demand and time loans by the method you choose (interest on limit, interest on outstanding, a share of the limit, spread over the remaining months, or not counted). You can untick any facility that will be closed or taken over, and compare the result with your bank's ceiling.

### Exports

* **Excel** workbook with Assessment, Contracts, Analytics, Monthly History, Summary and Data Checks sheets.
* **Print Summary**: one A4 page for the credit file.
* **Export HTML**: a full copy of all tabs.

### Several reports for one loan

Open the CIB reports of the applicant, co applicant and guarantor together and switch between them at the top of the page.

---

## Screenshots

All screenshots use made up sample data.

| | |
|---|---|
| ![Contracts](docs/screenshots/2_contracts.png) | ![Analytics](docs/screenshots/3_analytics.png) |
| ![DBR calculator](docs/screenshots/4_dbr_calculator.png) | ![Dark mode](docs/screenshots/5_dark_mode.png) |

---

## What CIBEX is not

CIBEX is **decision support only**. It reads the CIB report and lays out the facts. It gives **no risk score, no grade and no approve or decline**. Every bank has its own credit policy, and every credit decision remains with the underwriter and the bank.

Always check against the original CIB report and your bank's credit policy before relying on any figure. CIBEX is provided as it is, without warranty of any kind (see the licence).

---

## Testing

CIBEX was tested on more than 200 real CIB reports of individuals and companies, from small files to reports of several thousand pages. Its reading of every contract was checked against a separate reference reading. No customer report is included in this repository.

---

## Feedback

If CIBEX reads something wrongly, or you have an idea that would help your work, please open an issue on this page or send me a message on LinkedIn. Never attach a real customer's CIB report; describe the problem or use a masked copy.

---

## Licence

CIBEX is released under the MIT Licence. See [LICENSE](LICENSE).

CIBEX includes, unchanged, two open source libraries:

* **PDF.js** by Mozilla, Apache Licence 2.0 ([licence](third_party_licences/PDFJS_LICENSE.txt))
* **Chart.js**, MIT Licence ([licence](third_party_licences/CHARTJS_LICENSE.md))

---

**File check.** The SHA 256 of CIBEX_v1.0.html is listed in the [release notes](CHANGELOG.md), so you can confirm your copy has not been changed.
