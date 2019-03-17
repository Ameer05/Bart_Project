# Bart_Project

The objective of this assignment is to create a Python script which loads the BART data into your local database. In order to receive full credit on this assignment you will need to write a Python Script which takes the raw Excel files and prepocess them and loads in the clean ridership data.

### Things that we standardized:

* The format for year and month changes over time. Your code should standardize these changes. – The number of stations changes over time. If a particular file does not have a station, there is no need to add it.

* The daytypes (“Weekday”, “Saturday” and “Sunday”) change their names throughout the data. Make sure that they are standardized. You can ignore the phrase “adjustments.” The data was calculated the same way over the entire time period.

* Reshape the data from wide format into a long table. The data in the Excel spreadsheets is presented in a wide format – each column represents the average exits for a particular station. The target table (“cls.bart”) is long, not wide; the data will require reshaping before it is copied in.

## workflow
* Get list of fully qualified paths of files in root directory
* Unzip all files in zip_dir and store them in unzip_dir and get the list containing fully qualified paths of unzipped files
* Get month (int) and year (int) extracted from a string containing a month (name) and a year (numeric)
* Use the fully qualified path of a file with BART data to create a data frame with the ridership data in long table format
* Create a table in postgres using the information provided
* Get a list of the names of all columns in a postgres table
* Write all of the ridership data to a temporary csv file
* Send the ridership data from csv_file to a postgres table
* Clean and organize the BART ridership data and send it to a SQL db with SQLConn


 The project is under the instruction of Nick Ross as one of the projects of SQL class.
