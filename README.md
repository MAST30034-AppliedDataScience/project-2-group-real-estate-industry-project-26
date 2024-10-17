## MAST30034 Project 2 README.md
# Generic Real Estate Consulting Project
Group 26\
Group Member: Xuechun Cheng, Joel Antony, Yuchen Zhong, Mingqi Liu\
*-------------------------------------------------------------------\
**Research Goal:** The research goal is to discover the relationship between the price of rental properties and external and internal features, such as property type and living condition in the neighbourhood. Furthermore, discover the growth rate and livable level of each suburb.\

*-------------------------------------------------------------------\
1.'1.Scrape suburbs and postcode.ipynb'\
  **Description**: This jupyternotebook scraped all the suburb's name of Voctoria\
  **Output**: 'australian_postcodes.csv' in ***data/landing*** file

2.'2.Scrape Domain.ipynb'\
  **Description**: This jupyternotebook scraped 8000+ rental properties in Victoria\
  **Output**: 'properties.csv' in ***data/landing*** file

3.'3.scrape-additional.ipynb'\
   **Description**: This jupyternotebook scraped the public services in each suburb, such as hosipital, train station, etc.\
   **Output**:'park.csv', 'stations_and_suburbs.csv', 'victoria_shopping_centres.csv', 'hospital_health_services_addresses.csv' in ***data/landing*** file

4.'4.Data Preprocessing.ipynb'\
  **Description**: This jupyternotebook details all preprocessing steps of the main dataset 'properties.csv' and other additional dataset, and then combined them into a single dataset.\
  **notice** 'Crime.csv' and 'Criminal.numbers' is downloaded from 'https://www.crimestatistics.vic.gov.au/crime-statistics/latest-victorian-crime-data/download-data', since 'Criminal.csv' is too big and unable to uploaded it onto Github, therefore we upload it in 'Criminal.numbers' format, before using it you might need to transfer it into .csv form.\
  **Output**: 'LGA With Postcodes.csv', 'cleaned_hospital_health_services_addresses.csv', 'cleaned_park.csv', 'cleaned_properties.csv', 'cleaned_stations_and_suburbs.csv', 'cleaned_victoria_shopping_centres.csv',  'clean_data.csv', 'combined_data.csv', 'full_data.csv' in ***data/raw*** file 'final_data_full.csv', 'final_data_num.csv' in ***data/curated*** file

5.'5.past_data_clean.ipynb'\
  **Description**: This jupyternotebook details all preprocessing steps of the past dataset\
  **Output**: 'pased_data_clean.csv' in ***data/curated*** file

6.'6.Visualization.ipynb'\
  **Description**: This notebook is used to run the model and conduct analysis on the curated data\
  **Output**: Visualisation plot in data/plot file

7.'7.Growth Rate.ipynb'\
  **Description**: This notebook is used to run the model and predict the growth rate of each suburb.\
  **notice** 'POSTCODE_POLYGON.shp', 'POSTCODE_POLYGON.dbf', 'POSTCODE_POLYGON.shx' are downloaded from 'https://www.data.vic.gov.au/', 'australian_postcodes.csv' is downloaded from 'https://github.com/Elkfox/Australian-Postcode-Data/blob/master/au_postcodes.csv'.\
  **Output**: Growth rate prediction, plot in ***plot*** file

8. 'Summary.ipynb'\
   **Description**: This notebook provide a summary of the key points in our project. Includes code examples and a preview of the results，and the limitation & assumption we made during our working process.
