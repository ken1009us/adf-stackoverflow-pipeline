# Azure StackOverflow Data Pipeline

## Introduction
This repository contains a data processing workflow using Azure Data Factory (ADF) designed to extract question data from the StackOverflow REST API, process it, and store it in Azure Blob Storage.

## Architecture
This project implements a workflow to fetch, transform, and store data in different storage layers (landing, bronze, quarantine, silver).

### Pipelines
- **Ingest Pipeline**: Responsible for extracting data from the StackOverflow API.
- **Transformation Pipeline**: Handles data transformation.
- **Master Pipeline**: Manages overall workflow control and parameter passing.

### Datasets
- **Parquet Dataset**: Storage format for transformed data.
- **JSON Dataset**: Storage format for raw data from the API.

### Storage Folders
- **Landing**: Stores raw data fetched from the API.
- **Bronze**: Contains initially processed data.
- **Quarantine**: Stores data that does not meet quality standards.
- **Silver**: Stores cleaned and transformed data ready for analysis.

## Usage
Describe how to run and use this Data Factory configuration, including necessary Azure settings and any prerequisites.
