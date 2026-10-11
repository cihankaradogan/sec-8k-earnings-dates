# sec-8k-earnings-dates

Public SEC EDGAR data, re-published as plain CSV files so that a research backtest can download them.

- **Content:** the filing dates of Form 8-K / 8-K/A filings that report Item 2.02 ("Results of Operations and Financial
  Condition", i.e. an earnings release), by SEC CIK, 2010-01 .. 2019-01. Plus a list of periodic-report filers (CIK and
  last periodic filing), used to check coverage. No prices, no market data, nothing private.
- **Source:** SEC EDGAR bulk `submissions.zip` (https://www.sec.gov/Archives/edgar/daily-index/bulkdata/submissions.zip),
  downloaded with a declared User-Agent under SEC's fair-access rules. SEC EDGAR data is public.
- **Files:**
  - `qc1/selection_<sha12>.csv`: filings dated up to 2015-01-10 (columns `cik,filing_date`).
  - `qc1/qa/`: the full 2010-01 .. 2019-01 table and the filer list, for a counts-only coverage check.
- File names carry the first 12 hex digits of the file's SHA-256. The consumer verifies the full hash before use.

Provided as-is, with no warranty. Not investment advice.
