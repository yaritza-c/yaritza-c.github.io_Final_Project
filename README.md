# Final_Project

## Notes

### Communication

1. Using Slack for most communications
2. Meeting Mondays at 7 to prepare ourselves for the weekly meetings and segment deliverables

### Important Links

1. location of dataset: <https://www.consumerfinance.gov/data-research/hmda/historic-data/?geo=nationwide&records=all-records&field_descriptions=codes>
2. Google Slides presentation:







### 7/14/2022 Session

1. Cleaning the dataset
a) Dropping columns applicant_race_2 through applicant_race_5 and coapplicant_race_2 through coapplicant_race_5
b) respondent_id is index
c) add zeros to denied_reason_1 to indicate no denial (working)
d) drop denied_reason_2 and denied_reason_3 (working)

2. For segment 2 deliverables: Anu updating database (SQL); Alex, Victor, Olivia running machine learning models to determine most accurate model with small loss; Yaritza setting up presentation in Google Slides

NOTE: plz wait until we have a cleaned version of dataset before SQL and tableau use.

NOTE: hdma has an api

### 7/19/2022 Session

1. Additional Cleaning: All steps above were taken and...
a) removing outliers from the data under assumption that our dataset it normally distributed

2. Binning the data
a) Using the Action Taken column, add new column that condenses codes 1 and 6 to "Accepted", 4 and 5 to "Other", and 2, 3, 7, and 8 to "Denied." Drop "Other," and then This will be used as our output variable 

3. Once cleaned, (no null values), we will split the dataset into a smaller proportional sample (bc 14mil rows is not working on our computers)
a) decide on a number of sample csv's with proportions of output column similar to population (large csv)
b) current potential options: race/ethnicity (combine columns??), income bracket (bin), population size (bin), or agency type

4. In reference to the rubric, Anu is cleaning the model via SQL and will export new table for us to use. The data will be split into proportional groups based on choices (Alex?), run machine learning models (everyone?), reconvene and determine which models are working the best for the groups that we choose. What do we want to include in the presentation (Yartiza), create visualizations of our data in Tableau or something similar (Victor)

### 7/21/2022 Session

1. Running into issues with github storage, so to combat, we will only create important csv files, which will include...
a) machine learning model - proportional sample (based on action taken summary column)
b) visualization portion - income and loan amount binned (for analysis of columns)
c) hypothesis tests? - proportional sample (other variables yet to be determined like race, agency type, etc)
NOTE: original file is too large to get it on here

2. Create a cleaning file so that all that has to be done is run input file and it will automatically spit out a useful output file.




# Rubric Double Check

## Segment One

### Presentation

1. Selected Topic: Mortgage Loan Approval Calculator
2. Reason why topic is selected: Housing market is nuts, thus making it a topic of interest
3. Description of data source: hdma 2017 loan data
4. Questions we want data to answer: what variables most affect the approval of a mortgage

### Github

1. Include README: Done
2. README has description of the communication protocols: see above
3. Individual branches for each member: Done
4. Four commits from each member: probably impossible for segment 1

### Machine Learning Model

1. Take in data from provisional database: done
2. outputs labels for input data: loan approval is output and "several factors" for input

### Database:

1. sample data that mimics expected final database structure or schema: hmda 2017 nationwide; lending club?
2. Draft machine learning module is connected to the provisional database: working

## Segment 2

### Presentation

1. Description of the data exploration phase of the project
2. Description of the analysis phase of the project
3. Begin drafting slides in google slides

### Github

1. All code necessary to perfomr exploratory analysis in github
2. Some code necessary to complete machine learning portion





