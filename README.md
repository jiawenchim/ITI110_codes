Project information : Predicting London energy consumption 
- Data source: https://www.kaggle.com/datasets/jeanmidev/smart-meters-in-london?select=daily_dataset 

Project Resources:
Link to datasets folder: https://drive.google.com/drive/folders/1Cq7h4Hmq0wX9hR0EYbnfdOD47L9t0Pg2?usp=sharing
- "uk_bank_holidays.csv" : consists of public holiday date and information in UK
- "weather_daily_darksky.csv" : daily weather data in London
- "weather_hourly_darksky.csv" : hourly weather data in London
- "halfhourly_dataset.zip" : 112 csv files consisting 112 blocks data
- "concatenated_halfhourly_dataset.zip" : 1 csv file that concatenated all 112 blocks data (note: around 9GB large after unzipping)
- "2.2 merged_aggregated_hourly_without_block_id.csv" : Aggregated csv file (hourly) - use this for hourly prediction training (Label: avg_energy_per_lclid)
- "2.3 merged_aggregated_daily_without_block_id.csv" : Aggregated csv file (daily) - use this for daily prediction training (Label: avg_energy_per_lclid)

Notebooks in this Github repo : 
- 0 :  Codes used to concatenate the 112 csv files
- 1.2: for hourly energy consumption aggregation
- 1.3: for daily energy consumption aggregation
- 2: to merge aggregated hourly dataset with holiday and weather information
- 2.3: to merge aggregated daily dataset with holiday and weather information
- 3.1 to 3.5 : Custom LSTM models trainings
- 3.6 : Pretrained model NHiTS exploration

