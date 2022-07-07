# Election_analysis

## Overview
We are helping Tom audit the congressional election poll data for an election in Colorado. We used Python to read the data in a csv file containing the ballot ID, county, and candidate’s name. Then we used Python to calculate the total votes for each candidate and each county in which a vote was cast. Given this data, we were able to calculate the winning candidate, the percentage of votes they received, as well as the county with the most votes. This data was then stored in a new text file created by Python.

## Election Audit Results

There were a total of 369,711 votes cast in this election. Below are the overall results

### Counties
-	Jefferson: 38,855 votes (10.5%)
-	Denver: 306,055 (82.8%)
-	Arapahoe: 24,801 (6.7%)
Largest County Turnout: Denver

### Candidate votes
-	Charles Casper Stockham: 85,213 (23.0%)
-	Diana DeGette: 272,892 (73.8%)
-	Raymon Anthony Doane: 11,606 (3.1%)

As seen in the picture below, Diana Degette won.

![results.png](https://github.com/1fatpanda1/Election_analysis/blob/main/Resources/Winner%20results.png)

## Election-Audit Summary
The code used for this election could be used in any election given a few modifications. Assuming the input csv file was similarly organized, the biggest change probably be renaming the location variable names (for organisation) and outputs. For example, if we were tracking the US Presidential election, and we were tracking the states, one would change the largest county/county list variable/dictionary/list names to better match what sort of location we are tracking. Instead of county_options/county_votes/largest_county/etc. for variable and list names, one might choose to rename those state_options/state_votes/winning state, etc. Also, the output section would have to be changed from county (see below image) to state/nation/class or whichever demographic or area we are sorting by.
![example.png](https://github.com/1fatpanda1/Election_analysis/blob/main/Resources/example.png)

On the otherhand, if our csv inputs were ordered a bit differently, we would have to change which columns we are pointing at to store data as Python is going through each row. For example, maybe our csv file starts with county as the first column instead of Ballot id or there are additional columns, the following code would need to be adjusted such that county_name and candidate_name reference the correct column. 
![rowcountcode.png](https://github.com/1fatpanda1/Election_analysis/blob/main/Resources/row%20count.png)
