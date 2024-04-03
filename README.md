# AWS-Dynamodb-Data-Manipulation

# DynamoDB Data Management Scripts

## Overview

This project comprises Python scripts designed to interact with Amazon DynamoDB, a NoSQL database service provided by AWS. These scripts enable various data management tasks such as creating tables, inserting, updating, querying, and deleting items in DynamoDB tables.

## Prerequisites

- Python 3.x installed on your system.
- `boto3` library for AWS SDK for Python. Install it using pip:

    ```
    pip install boto3
    ```

- Ensure that you have the necessary permissions and credentials configured for accessing AWS services.

## Scripts

### 1. `dynamodb_data_management.py`

This script contains functions for performing CRUD (Create, Read, Update, Delete) operations on a DynamoDB table named "Movies". It includes functions to:

- Create a DynamoDB table named "Movies".
- Insert an item into the "Movies" table.
- Update an item in the "Movies" table.
- Conditionally update an item in the "Movies" table based on a condition.
- Retrieve an item from the "Movies" table.
- Delete an item from the "Movies" table.
- Insert sample movie data into the "Movies" table.
- Query movies released in a specific year.
- Query movies with additional conditions (e.g., released in a specific year and having titles starting with certain alphabets).
- Scan the entire "Movies" table for items based on a filter condition.

## Usage

1. Ensure you have the required libraries installed as mentioned in the Prerequisites section.
2. Configure AWS credentials on your local machine.
3. Run the `dynamodb_data_management.py` script using Python:

    ```
    python dynamodb_data_management.py
    ```

4. The script will execute all the defined functions sequentially, performing various data management tasks on the DynamoDB "Movies" table.

## Notes

- Ensure that your AWS credentials have the necessary permissions to create, read, update, and delete items in DynamoDB tables.
- Review the script and modify the AWS region and endpoint URL as per your DynamoDB setup if needed (currently set to "eu-west-1" and "http://localhost:8000" respectively for local DynamoDB usage).
- Customize the script to suit your specific DynamoDB table schema and data management requirements.

