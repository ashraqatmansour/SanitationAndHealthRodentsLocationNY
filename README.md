# NYC Rodent Complaints by Building Type

## Project Overview

This project analyzes NYC public health complaint data to identify **building structure types most frequently associated with rodent infestations**. By filtering complaints within a user-specified date range and aggregating results by location type, the project highlights environmental and structural risk factors relevant to **urban public health and housing conditions**.


## Process

- Analyze NYC public health data to identify building types most associated with rodent complaints  
- Clean, filter, and aggregate large datasets to extract meaningful patterns  
- Visualize results to highlight structural and environmental risk factors  

## Data Description

The input dataset is a CSV file containing NYC rodent complaint records, including:
- Created Date  
- Location Type (building or structure type)  

The analysis focuses on complaints that fall within a specified date range.

## Script 1: Data Aggregation (Python)

This script:
- Accepts an input CSV file and a date range
- Filters complaints by date
- Counts the number of rodent complaints per building type
- Outputs results to a CSV file or standard output

### Usage

bash
python building_type_counts.py \
    --input_file data.csv \
    --start_date YYYY-MM-DD \
    --end_date YYYY-MM-DD \
    --output_file building_count.csv

## Output Format
Building Type,count
Residential Building,1234
Commercial Building,987
Mixed Use,654

## Script 2: Data Visualization

The visualization script:

Reads the aggregated CSV output

Identifies the top 10 building types with the highest rodent complaint counts

Displays a horizontal bar chart for easy comparison

## Visualization Output

<img width="837" height="480" alt="Screenshot 2026-01-12 at 12 28 08 PM" src="https://github.com/user-attachments/assets/6f8c9300-d30a-408d-8681-57f0b68208cc" />


## Tools and Technologies

Python

CSV and argparse modules

Pandas

Matplotlib
