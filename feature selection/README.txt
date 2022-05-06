=== General Information ===
The feature selection folder contains Jupyter Notebook files used to analyze bus data features.
Different get_correlations files were used for different routes because the orginal data for each route was different. Routes 187 and 188 had similarly formatted data, so 1 script was used for both. 
Datasets of the same route were formatted the same and included the same columns. 
The files remove all non-numerical columns, then find the correlation for each remaining column with the current departure offset, and output the correlations as a csv file. 
Different route datasets have different columns that needed to be removed.
These csv output files can be found in the "data" folder. 

=== feature selection File Descriptions === 

2019_feature_selection.ipynb			correlation between various features and current departure offset. Previous departure offset, operating speed, Miles from prior timepoint, inverse dwell time. graphs included
Get_Correlation_For_Line280.ipynb		finds correlation for all features and "Difference (Minutes)" aka current departure offset; output file "data\2020 Line 280 correlations.csv" also 2019 280 correlations file
get_correlation_for_silverstreak.ipynb	get_correlations file edited to produce similar csv file for silver streak data
get_correlations.ipynb				used for 187 188, finds correlation for for all features and "Difference (Minutes)" aka current departure offset, outputs as csv


Last updated: 5/5/22	Daniel Uyematsu