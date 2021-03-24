# Historical CDC Vaccination Time Series Data
Source: https://covid.cdc.gov/covid-data-tracker/#vaccinations

*Updated daily minus holidays*

Visualization of CDC data available at [covid19-projections.com](https://covid19-projections.com/path-to-herd-immunity/).

## Raw Endpoints

Below are the raw API endpionts that we use to download and save the data daily:

- Vaccinations: https://covid.cdc.gov/covid-data-tracker/COVIDData/getAjaxData?id=vaccination_data
- Trends (New since 2021-02-03): https://covid.cdc.gov/covid-data-tracker/COVIDData/getAjaxData?id=vaccination_trends_data

## Files

- `aggregated.csv` - Raw/unedited CDC vaccination time series data, aggregated from daily CDC updates. Starts from 2020-12-20 for US nationwide and 2020-12-30 for all states. Missing dates mean that there were no CDC updates on those dates.
- `aggregated_adjusted.csv` - Adjusted time series data to account for missing days/entries. All lower-case columns are not in the original dataset. Column names should be self-explanatory. Feel free to [open an issue](https://github.com/youyanggu/covid19-cdc-vaccination-data/issues) with any questions/comments/bugs.
- `cdc_vaccination_trends_data.csv` - Raw US and Long-Term Care time series vaccination data (newly released [by the CDC](https://covid.cdc.gov/covid-data-tracker/#vaccination-trends) on 2021-02-03)

## Other Repositories

- [Main COVID-19 Repository](https://github.com/youyanggu/covid19_projections)
- [Infections Estimates](https://github.com/youyanggu/covid19-infection-estimates-latest)
- [COVID-19 Datasets](https://github.com/youyanggu/covid19-datasets)
- [SEIR Simulator](https://github.com/youyanggu/yyg-seir-simulator)
- [Model Evaluations](https://github.com/youyanggu/covid19-forecast-hub-evaluation)
