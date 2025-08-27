1. Data Import & Cleaning Context
* You use read_csv() already, but maybe show contrast with read_excel() or readr vs. base R functions.
* Include janitor::clean_names() explicitly early on so students see how to standardize messy column names.
2. Handling Data Types
* Show how to convert character to numeric, factors, or dates (as.numeric(), as.Date(), lubridate for sports timelines).
* Demonstrate dealing with inconsistent text entries (e.g., “OKC” vs “Oklahoma City Thunder”).
3. Joins Beyond full_join()
* Briefly compare inner_join(), left_join(), anti_join() with examples. Sports data often requires semi/anti joins (e.g., “players who appear in one dataset but not another”).
4. Data Reshaping (tidyr)
* Show how to use pivot_longer() / pivot_wider() when transforming raw box score formats.
* Example: making per-quarter stats long-form for analysis.
5. Case_when() for Conditional Mutations
* Very useful for creating categorical variables, such as grouping positions into “Guard / Forward / Center.”
6. Strings & Regex
* stringr functions (str_detect, str_replace) are often essential in wrangling sports data (e.g., cleaning player/team names).
7. Exploratory Wrangling Helpers
* count() for quick frequency tables.
* distinct() to drop duplicates.
* slice_max() and slice_min() as alternatives to arrange+head.
9. Efficiency & Workflow Tips
* Mention %<>% from magrittr for assignment-in-place.
* Encourage chaining multiple steps in a single pipeline for readability.
* Highlight RStudio shortcuts and how to debug when pipes get long.
10. Practice Opportunities
* After each verb, add a “Now you try” exercise (e.g., “Filter players with > 500 rebounds” or “Find top 3 teams by average assists”).
