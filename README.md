# Fitness Zone Analyzer

This website calculates annual aggregate FitnessGram Healthy Fitness Zone results from a WELNET export without uploading or saving student rows.

## Use

1. Open `index.html` in a modern browser, or publish it with GitHub Pages.
2. Export the source data from Google Sheets or Microsoft Excel as `.xlsx`, `.xls`, or `.csv`.
3. Upload the file and review the automatically detected categories.
4. Select **Analyze the School Year**.
5. Review Annual, Latest, Pre, Post, and Pre-to-Post movement totals.
6. Print the summary or download the aggregate Excel report.

The site discards individual spreadsheet rows immediately after calculating totals. It does not use cookies, local storage, a database, analytics, or a server upload. Excel parsing uses SheetJS loaded from jsDelivr. CSV analysis can work without that library.

## Expected fields

Grade, age, gender, and phase are required. Boys and girls may be included in the same file. The site supports curl-ups, 90-degree push-ups, trunk lift, combined left/right back-saver sit-and-reach, combined shoulder stretch, 15-meter and 20-meter PACER, one-mile run, and flexed-arm hang.

Use `M` or `F` for gender and `Pre`, `Mid`, or `Post` for phase. One-mile times can use `minutes:seconds`, such as `10:30`. Combined left/right values may use a pipe, such as `9 | 10`. `X`, `M`, blank, invalid, and adapted entries such as `A12` are excluded from HFZ calculations.

Annual means the student met a category's HFZ at least once during the school year. Latest uses Post when available, then Mid, then Pre. If a student has only one valid assessment, it becomes both the Annual and Latest result. Pre-to-Post movement is reported separately.

## Standards and limits

When a WELNET export contains matching `Standard Met` columns, the website uses WELNET's `Y` and `N` results as the authority. A blank WELNET status is treated as not scored. The embedded 2007 FitnessGram Healthy Fitness Zone tables are used only when the corresponding WELNET status column is absent.

Confirm the standards and assessment rules required by your district before using the totals for official reporting. FitnessGram advises against using these results to grade individual students, compare students with one another, or evaluate teacher effectiveness.
