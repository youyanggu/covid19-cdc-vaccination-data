# Historical CDC Vaccination Data
https://covid.cdc.gov/covid-data-tracker/#vaccinations

Updated daily (or as often as CDC updates their data, which should be daily minus holidays).

## Files

- `aggregated.csv` - Raw/unedited CDC vaccination data. Starts from 2020-12-20 for the US and 2020-12-30 for all states. Missing dates mean there were no CDC updates on that day.
- `aggregated_adjusted.csv` - Adjusted data to account for missing days/entries. All lower-case columns are not in the original dataset. Column names should be self-explanatory. Feel free to open an Issue with any questions.
