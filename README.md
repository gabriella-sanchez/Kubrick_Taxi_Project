# Kubrick_Taxi_Project
A project to develop automated pipelines that will populate fact table(s) and dimension tables for NYC taxi data

The NYC Taxi and Limousine Commission has a public record of vehicle journeys in the NY area:
Your task:
Develop automated pipelines that will populate fact table(s) and dimension tables.
The suggested approach (and this is only a suggestion, it may more complex) is as follows:
1. Copy the data to Azure storage and then transform the data in Snowflake.
2. Create some dimension tables and populate the reference data for Rate codes, Payment types and Taxi
zone names.
3. Create a dimension load pipeline in Azure Data Factory to load the taxi+_zone_lookup.csv file to
populate the Zone dimension. Consider how you would handle rate codes and payments changes. You
need to handle this in your automated pipeline.
4. Create some suitable table structures for the trip data. The yellow/green trip data can go into the same
fact table. Differentiate the two in the fact table with a Trip Type dimension key.
5. Create some “staging” tables for the trip data. The usual approach is usually to load each file of data
into the staging tables first, then insert it into the target tables.

Additional Tasks:
Your Agile project should be structured and run according to accepted best practice.
i.e
Daily standups and other rituals
use of repos to securely manage your code.
use of Azure DevOps or similar
