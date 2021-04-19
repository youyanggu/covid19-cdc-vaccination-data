# Historical CDC Vaccination Time Series Data
Source: https://covid.cdc.gov/covid-data-tracker/#vaccinations

**April 19, 2021 Update:** We added raw CSV files to the [`raw_csv`](/raw_csv) directory. These are the raw vaccination data released by the CDC on each date (no look-ahead bias).

From December 2020 to March 2021, we aggregated daily vaccination snapshots from the [CDC Vaccinations](https://covid.cdc.gov/covid-data-tracker/#vaccinations) page. We make this time series data available in this repository. This is different than the [CDC Vaccination Trends](https://covid.cdc.gov/covid-data-tracker/#vaccination-trends) data, as that dataset is retroactively updated based on the date of vaccination, whereas this one is based on date of reporting and hence is not retroactively updated. Hence, for model training, we recommend using this non-retroactive dataset to avoid look-ahead bias.

Visualization of CDC data available at [covid19-projections.com](https://covid19-projections.com/vaccination_cdc) (through March 8, 2021). Learn more about how *covid19-projections.com* used this data on the [Path to Normality](https://covid19-projections.com/path-to-herd-immunity) page.

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
