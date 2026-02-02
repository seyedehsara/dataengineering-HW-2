# dataengineering-HW-2

1. Within the execution for Yellow Taxi data for the year 2020 and month 12: what is the uncompressed file size (i.e. the output file yellow_tripdata_2020-12.csv of the extract task)?
answer : 134.5 MiB

2. What is the rendered value of the variable file when the inputs taxi is set to green, year is set to 2020, and month is set to 04 during execution?
   answer : green_tripdata_2020-04.csv

3. How many rows are there for the Yellow Taxi data for all CSV files in the year 2020?

answer : 

SELECT count(*) 
FROM `project_id.taxi_dataset.yellow_tripdata` 
WHERE EXTRACT(YEAR FROM tpep_pickup_datetime) = 2020;;

24,648,499

4. How many rows are there for the Green Taxi data for all CSV files in the year 2020?

answer : 

SELECT count(*) 
FROM `project_id.taxi_dataset.green_tripdata` 
WHERE EXTRACT(YEAR FROM tpep_pickup_datetime) = 2020;


1,734,051

5. How many rows are there for the Yellow Taxi data for the March 2021 CSV file?

answer : 

SELECT count(*) 
FROM `project_id.taxi_dataset.yellow_tripdata`
WHERE filename = 'yellow_tripdata_2021-03.csv';

1,925,152

6. How would you configure the timezone to New York in a Schedule trigger?

answer : 
Add a timezone property set to America/New_York in the Schedule trigger configuration 
