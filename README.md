# ptab_project

This repository contains an analysis of decisions by the [Illinois Property Tax Appeal Board (PTAB)](http://www.ptab.illinois.gov/).


There are three primary scripts.

## Extracting Data
This script scrapes the PTAB website to find all recent decisions, downloads the decisions as PDFs, and then extracts metadata and text into a database.

About 122,500 pdfs were successfully downloaded and extracted. 

## Building Standardized Data
This script processes the raw extracted data into a cleaned file suitable for analysis. The data is highly structured, but a series of logic gates were necessarily to ensure data was consistent. Out of about 46,000 decisions which had hearings, 45,700 were able to be processed.

## Modeling Data
This script takes the processed data and trains and produces results based on the framework from Homework 2. This script also produces accuracy based on data subsets from non-text characteristics (e.g. County, Year, or Property Type)

