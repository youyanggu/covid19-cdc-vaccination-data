# Historical CDC Vaccination Data
Source: https://covid.cdc.gov/covid-data-tracker/#vaccinations

*Updated daily minus holidays*

Visualization of CDC data available at [covid19-projections.com](https://covid19-projections.com/path-to-herd-immunity/).

## Files

- `aggregated.csv` - Raw/unedited CDC vaccination data. Starts from 2020-12-20 for US nationwide and 2020-12-30 for all states. Missing dates mean that there were no CDC updates on those dates.
- `aggregated_adjusted.csv` - Adjusted data to account for missing days/entries. All lower-case columns are not in the original dataset. Column names should be self-explanatory. Feel free to open an Issue with any questions.

## Other Repositories

- [Latest Infections Estimates](https://github.com/youyanggu/covid19-infection-estimates-latest)
- [Main Data Repository](https://github.com/youyanggu/covid19_projections)
- [COVID-19 Datasets](https://github.com/youyanggu/covid19-datasets)
- [SEIR Simulator](https://github.com/youyanggu/yyg-seir-simulator)
- [Model Evaluations](https://github.com/youyanggu/covid19-forecast-hub-evaluation)
