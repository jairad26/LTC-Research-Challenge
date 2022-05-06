=== Dataset Information ===
The data folder contains all of the original and modified datasets that were used. Routes 707 (aka Silver Streak), 187, and 188 have data for 2019, 2020, and 2021. Route 280 data 
	was received from Foothill transit first and is only from the years 2019 and 2020. 280 2021 data was not available. 
The original datasets needed to be modified to be readible (chronological order, stops of same trip grouped together, etc.). Original datasets were sometimes in reverse order or 
	were split into different Excel sheets by month. Modified datasets were created by editing the original datasets in Excel or with a python script, whichever was easiest. 


=== data File Descriptions === 

original data					initial Foothill Transit datasets
187 188 Correlations.xlsx			every feature's correlation with "Difference (Minutes)" for route 187 and 188 in 2019, 2020 and 2021. This file comprises the other 6 
								correlation output files for 187 and 188. In columns D and E, features are reordered from highest to lowest correlation
2019 Line 187 allscripts.csv			187 2019 data organized by date, then block #, then time, with added columns Actual Depart, Actual Depart Hour, Prev Departure Offset
2019 Line 187 correlations.csv		correlations for 187 2019, output file from "feature selection/get_correlations.ipynb"
2019 Line 188 allscripts.csv			188 2019 data organized by date, then block #, then time, with added columns Actual Depart, Actual Depart Hour, Prev Departure Offset
2019 Line 188 correlations.csv		correlations for 188 2019, output file from "feature selection/get_correlations.ipynb". 
2019 Line 280 AVL allscripts.csv		280 2019 data with Same Stop Prev Trip Departure Offset and Transit Date Month, builds from "2019 Line 280 AVL prevdepoffset.csv"
2019 Line 280 AVL prevdepoffset.csv		280 2019 data with previous departure offset column added
2019 Line 280 correlations.csv		correlations for 280 2019, output file from "feature selection/get_correlations.ipynb"
2019 Silver Streak allscripts.csv		707 2019 data organized by date, then block #, then time, with added columns Actual Depart, Actual Depart Hour, Prev Departure Offset
2019 Silver Streak Correlations.csv		correlations for 707 2019, output file from "feature selection/get_correlations.ipynb"
2019 Silver Streak prevdepoffset.csv	707 2019 data with previous departure offset column added

2020 and 2021 files similar to 2019 files shown above. 

raw_data_to_allscripts.ipynb			adjusted to modify original datasets to readable format, outputed allscripts and prevdepoffset csv files as needed. 

Last updated: 5/5/22	Daniel Uyematsu