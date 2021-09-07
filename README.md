# Election Result Audit
## Overview

Using data provided by the Colorado Board of Elections, I analyzed the results of a recent congressional election held in Colorado. This analysis determined the voter turnout for this election and also provided a breakdown of turnout by county to determine which county casted the most votes for this election. This analysis also provided a breakdown of the election results in order to determine the winning candidate.

### Election Results

#### Turnout

This analysis counted the total number of votes and the breakdown by county. In this election, 369,711 voters participated. The turnout by county was as following:

- Jefferson County: 10.5% of the total vote (38,855 votes)
- Denver County: 82.8% of the total vote (306,055 votes)
- Arapahoe County: 6.7% of the total vote (24,801 votes)

Based on these figures, the largest share of the voter turnout came from Denver county.

#### Candidates

This analysis also counted the number of votes for each candidate: The results were as following:

- Charles Casper Stockham: 23.0% of the total vote (85,213 votes)
- Diana DeGette: 73.8% of the total vote (272,892 votes)
- Raymon Anthony Doane: 3.1% of the total vote (11,606 votes)

Based on these figures, Diana DeGette won the election with 272,892 votes, which represents 73.8% of the total vote.

### Audit Summary

While this script was used specifically to analyze the results of an election in Colorado, it can easily be modified to analyze the results of any election.

![load_data_code_screenshot](https://github.com/teruki-i/election_audit/blob/29289740c41525837d30a9b659bb58446da86a14/Resources/script_screenshots/load_data.png)

Line 9 of this script has a line of code that loads the data file for the election results from a file path. If another data file has data from another election organized in the same structure as the file used for this analysis, then the file path indicated in the join function would just have to be modified to that of the second data file.

A few cosmetic modifications can be made. This script also creates print statements for the results by county and thus print out "County" as part of the statements. 

![print_statement_code_screenshot1](https://github.com/teruki-i/election_audit/blob/main/Resources/script_screenshots/print_statement_1.png)
![print_statement_code_screenshot2](https://github.com/teruki-i/election_audit/blob/main/Resources/script_screenshots/print_statement_2.png)
![print_statement_code_screenshot3](https://github.com/teruki-i/election_audit/blob/main/Resources/script_screenshots/print_statement_3.png)

These could easily be modified to be applicable to different types of muncipal entities, such as cities. The word "County" in the lines of code for these print statements (though not necessarily the ones within the curly brackets)** would simply have to be replaced with the word "City."

**In this script, the word "county" appears in the variable names. Though not strictly necessary, when creating a modified version of this script to print city results rather than county results, in order to avoid confusion, it would be best to also modify the variable names to refer to cities rather than counties.