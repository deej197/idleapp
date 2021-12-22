# idleapp

**Motivation**:
Python is very handy language than can be used to automate repetitive tasks like report generation for business reviews. In support industry, tickets are logged and customers are alligned engineers to work with them until the issue is resolved. Customer satisfaction is very important for any successful business. Besides providing quicker resolution, keeping customers updated regarding the progress of the case is really essential.

To ensure that customers are informed and kept updated, identifying if the ticket is idle or not is really essential. This tool will read the input file and identifies if the ticket is idle or not using the last communication date. if the previous communication was sent before 5 days of time, it will mark the ticket as idle.

This idleapp.exe is built from a python script which can read data from .xlsx files and outputs the report in a .xlsx file with charts and table.

**How to run the .exe and generate output:**
Inside dist folder, doubleclick on idleapp.exe. It will prompt for input file name.
I have added input file in the same directory as inputdata.xlsx. Enter the input file name with inputdata.xlsx
And this will publish the output in result.xlsx

**Technical information:**
python packages such as numpy, pandas have been used for reading and processing input data from excel.
There was basic data preprocessing done to get the calculate the idle days as the date was in different format.
Used XlsxWriter https://pypi.org/project/XlsxWriter/ to create reports with charts and table in excel.
Used pyinstaller module https://pypi.org/project/pyinstaller/ to convert .py to .exe, so that the tool can run on devices without python installed.
