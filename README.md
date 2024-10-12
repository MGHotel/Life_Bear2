# Life_Bear
MG
README: Data Cleaning Script
Purpose:
This Python script is designed to clean a CSV file named chunk_10.csv. It performs the following tasks:

Reads the CSV file: Loads the data from the specified CSV file into a pandas DataFrame.
Checks for email column: Verifies if the DataFrame contains an 'email' column.
Drops null values: Removes rows with null values in the 'email' column, if it exists.
Validates email addresses: Identifies and removes rows with invalid email addresses based on a regular expression pattern.
Saves invalid rows: Creates a dump file named invalid_rows_dump.csv to store rows with invalid email addresses.
Usage:

Prerequisites: Ensure that the required libraries (pandas and re) are installed.
File Placement: Place the script and the CSV file (chunk_10.csv) in the same directory.
Run the script: Execute the script using a Python interpreter.
Output:

Cleaned DataFrame: The script will print the cleaned DataFrame to the console.
Invalid Email Rows: The script will print the rows with invalid email addresses to the console and save them to the invalid_rows_dump.csv file.
Customization:

File Path: Modify the file_path variable to specify the path to your CSV file.
Email Validation: Adjust the regular expression pattern in the is_valid_email function to customize email validation criteria.
Dump File: Change the dump_file_path variable to specify a different location for the dump file.
Notes:

The script assumes that the CSV file has a header row.
If the 'email' column does not exist in the DataFrame, the script will skip dropping null values and email validation, but it will still create an empty dump file.
For more complex cleaning tasks, consider using additional libraries like NumPy or specialized data cleaning tools.
