# 2020_three_us_communities_coc_homeless_counts
This .csv format dataset contains the point-in-time information about the homeless counts for three communities in January 2020. Specifically, the data about the New York City was collected on 1/27/2020, the data about the Los Angeles City & County was collected on 1/22/2020, and the data about the Seattle and King County was collected on 1/23/2020.

The intended audience is investigative or reporting journalists who have the needs of drawing upon empirical evidence for writing a comparative story about the homeless populations among different U.S. Cities and Counties for the public to know. 

The dataset is designed to help journalists collect evidence to do comparative news writing about the homeless counts among three U.S. communities. Data curation process is described as below:
1.	The dataset was created from the Continuums of Care (CoC) Homeless Populations and Subpopulations Reports of the three U.S. communities (New York City, Los Angeles City & County, Seattle and King County). The reports are open source, freely available to the public on the HUD Exchange website.
2.	Then, to help journalists focus on the comparisons of homeless counts, this dataset extracts the most relevant data points (total homeless households, total homeless persons of the three communities) from the original three CoC reports and adds them to this dataset.
3.	To emphasize the homeless counts are the point-in-time counts, this dataset adds a field to record the date that the point-in-time counting happened. This would enable journalists to have more context about what these homeless counts exactly refer to and how to properly compare these counts considering other contextual factors. 
4.	To help journalists understand a larger picture instead of just one point-in-time picture, this dataset also extracts the total numbers of the chronically homes households and the chronically homeless persons from the original three CoC reports.
5.	To help journalists compare the ratio of the homeless population among these three communities, this data extracts the data about the total population counts of all the three communities from the QuickFacts data, which is freely available to the public on the census.gov website.
6.	The file naming convention is: year_datasettype. The year indicates the year in which the point-in-time count occurred. The dataset type indicates whether the dataset is the raw data ("raw") or the normalized data ("normal").

## Data Dictionary
|Variable |Variable Name  |Measurement Unit  |Allowed Values  |Definition  
--- | --- | ---| --- | --- |
|CoC Community Code|Coc_Report|String|CoC codes|The code number of the CoC community Field Office|
|CoC Community Name|Community_Name|String|New York City, Los Angeles City and County, Seattle and King County|The names of the CoC communities|
|Point-In-Time Counts Date|Point_In_Time_Date|Date|MM/DD/YY|Date of the point-in-time homeless counts|
|Total Point-In-Time Homeless Households Counts|Total_Homeless_Households|Numerical|Number >= 0|The total count of point-in-time homeless households of the corresponding community|
|Total Point-In-Time Homeless Persons Counts|Total_Homeless_Persons|Numerical|Number >= 0|The total count of point-in-time homeless persons of the corresponding community|
|Total Chronically Homeless Households Counts|Total_Chronical_Homeless_Households|Numerical|Number >= 0|The total count of the chronically homeless households of the corresponding community|
|Total Chronically Homeless Persons Counts|Total_Chronical_Homeless_Persons|Numerical|Number >= 0|The total count of the chronically homeless persons of the corresponding community|
|Total Population|Population|Numerical|Number >= 0|The total count of population in the corresponding community|
