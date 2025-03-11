# Climate Data Analysis with AWS

This project demonstrates how to analyze global land temperatures using AWS data engineering tools.

## Dataset

The project uses the Berkeley Earth Climate Change: Earth Surface Temperature Data dataset, which contains monthly average land temperatures for various cities and countries around the world.

## AWS Services

* S3: Stores the raw and cleaned data.
* Glue: Crawls the data in S3 and creates metadata in the Glue Data Catalog.
* Athena: Queries the data in the Data Catalog.
* QuickSight: Visualizes the cleaned data.

## Steps

1.  **Data Ingestion:** The raw data is uploaded to an S3 bucket.
2.  **Data Cataloging:** A Glue crawler is used to create metadata for the data in the Glue Data Catalog. This step ensures that the data is easily discoverable and queryable. The crawler's logs provide valuable insights into the data's structure and any potential inconsistencies.
3.  **Data Cleaning and Transformation:** SQL queries are used in Athena to clean and transform the data, including handling missing values and removing unnecessary columns.
4.  **Data Visualization:** QuickSight is used to create an interactive dashboard that visualizes the cleaned data.

## Key Findings

* The analysis revealed a clear warming trend in global land temperatures over the past century.
* Regional variations in temperature patterns were also observed.



## Links

* Berkeley Earth dataset: \[https://www.kaggle.com/datasets/berkeleyearth/climate-change-earth-surface-temperature-data](https://www.kaggle.com/datasets/berkeleyearth/climate-change-earth-surface-temperature-data)
