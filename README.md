# Fitness Zone Analyzer

This website calculates aggregate FitnessGram Healthy Fitness Zone results without uploading or saving student rows.

## Use

1. Open `index.html` in a modern browser, or publish it with GitHub Pages.
2. Export the source data from Google Sheets or Microsoft Excel as `.xlsx`, `.xls`, or `.csv`.
3. Upload the file and confirm the column mapping.
4. Select **Analyze Fitness Zones**.
5. Print the summary or download the aggregate CSV.

The site discards individual spreadsheet rows immediately after calculating totals. It does not use cookies, local storage, a database, analytics, or a server upload. Excel parsing uses SheetJS loaded from jsDelivr. CSV analysis can work without that library.

## Expected fields

Grade, age, and sex are required. The site supports curl-ups, 90-degree push-ups, trunk lift, left and right back-saver sit-and-reach, left and right shoulder stretch, 15-meter and 20-meter PACER, one-mile run, and flexed-arm hang.

Use `M` or `F` for sex. One-mile times can use `minutes:seconds`, such as `10:30`. Shoulder stretch values can use `Yes` or `No`. `X`, `M`, blank, invalid, and adapted entries such as `A12` are excluded from HFZ calculations and reported as **Not Scored**.

## Standards and limits

The embedded thresholds follow the 2007 FitnessGram Healthy Fitness Zone tables for boys and girls supplied with this project (Tables 9.1 and 9.2). Scores at or above the lower HFZ value count as meeting the standard; one-mile times at or below the listed time count as meeting the standard. Aerobic criterion standards are unavailable for ages 5 through 9, except that a 9-year-old in grade 4 may be evaluated using the age-10 standard.

Confirm the standards and assessment rules required by your district before using the totals for official reporting. FitnessGram advises against using these results to grade individual students, compare students with one another, or evaluate teacher effectiveness.
