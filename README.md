# Evolution PE Fitness Test Analyzer (beta)

A single web page (`index.html`) that summarizes class fitness-testing results. It runs in your browser. It does not upload, save, or send student rows anywhere, and it has no cookies, accounts, or analytics.

## Use
1. Open `index.html` in a modern browser, or publish the repo with GitHub Pages.
2. **Step 1:** choose the standards: your FitnessGram "Standard Met" columns, the 2026 Presidential Physical Fitness Test benchmarks, or your own standards.
3. **Step 2:** add scores by **uploading a file** (.xlsx, .xls, .csv) or by **typing or pasting scores**.
4. Review what was found, choose **Analyze**, then print the report or download the Excel summary.

## Typing or pasting scores
- **Paste straight into the table.** Copy cells from Excel or Google Sheets, click the first **Student ID** box, and paste. The cells land in the right columns, and new rows are added as needed.
- **Headings are optional.** With a heading row, columns can be in any order (Gender or Sex, Mile, Pushups, etc.). Without one, columns are read in the order of the table; the paste box shows that order.
- Words are understood: Boy/Girl or Male/Female, "4th" or "K", "pre".
- **Mile times:** type `830` and it becomes `8:30`. Spreadsheet time cells such as `0:08:30` and `8:30:00` are read as 8:30. Decimal times such as `8.30` are **not guessed**; you are asked to change them to `8:30`, because they could be misread as 8 minutes 18 seconds.
- On phones, score boxes open a number keypad.
- Use initials or ID numbers, not student names. Nothing is saved; use **Download my table (CSV)** before closing the page.

## Version 2.1 changes (typing and pasting)
- Pasting a block into the table no longer dumps everything into one box.
- Spreadsheet time cells are no longer silently left out.
- Decimal mile times are no longer silently misread.
- Heading row is optional in the paste box.
- Uploads give identical results to version 2 (checked with a 24-row sample).

## Not yet verified
- **The built-in FitnessGram tables are copies of FitnessGram standards.** Ask the Cooper Institute and GreenLight Fitness before sharing widely. The PACER numbers were read from screenshots; check them against the official chart. The older 2007 tables were not re-checked.
- Tested in desktop Chrome and a phone-size window. Not tested on a real phone, Safari, or a screen reader.
- The Presidential table does not say which beep-test recording its lap counts assume.
- Uploads of mile times written as decimals (such as `8.30`) are still read as decimal minutes. Use `m:ss`.

## Important
- Do not use identifiable student data until your district approves it. Follow your district's rules.
- Independent tool. Not affiliated with or endorsed by The Cooper Institute, GreenLight Fitness (WELNET), or the President's Council on Sports, Fitness & Nutrition. FITNESSGRAM and Healthy Fitness Zone are registered trademarks of The Cooper Institute.

## Rollback
The previous version is in the commit history. Restore `index.html` from the commit before "Fitness Test Analyzer 2.1".
