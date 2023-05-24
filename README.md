# Insurance_Data_Analysis


This Python script is designed to perform analysis on insurance data stored in multiple files. The script utilizes various libraries such as numpy, pandas, matplotlib, and seaborn for data manipulation, visualization, and analysis.


# Installation

Clone the repository or download the script file.
Ensure that you have Python installed on your system.
Install the required libraries by running the following command:
" pip install numpy pandas matplotlib seaborn "

# Usage
Open the script in a Python IDE or text editor.
Modify the file paths in the code to match the location of your data files.
Run the script.


The script performs the following operations:

- Changes the current working directory to the specified project directory.
- Reads the frequency data from the db_freq.xlsx file into a pandas DataFrame (freq).
- Sorts the freq DataFrame by the IDpol column in ascending order.
- Reads the severity data from the db_sev.txt file into a pandas DataFrame (sev).
- Reads the premium data from the db_prem.csv file into a pandas DataFrame (prem).
- Sorts the prem DataFrame by the IDpol column in ascending order.
- Calculates the number of duplicate IDpol values in these DataFrames.
- Displays the duplicate IDpol values in the prem DataFrame.
- Calculates the number of missing values (NaN) in the sev DataFrame.
- Calculates the total number of missing values in the prem DataFrame.
- Imputes missing values in the VehPower column and VehGas column of the prem DataFrame using the mode.
- verification and identification of inconsistent data in dataframes
- The merge() function is used to merge the prem_ssDMDI and freq DataFrames on the 'IDpol' column, performing an inner join.
