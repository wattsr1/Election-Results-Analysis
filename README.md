# Election Summary

## Overview
This project was developed to create a python script to automate the process of auditing the votes and provide a summary that can be submitted to the Election's Board.  The data for each polling location is stored in a comma seperated values(CSV) file which identifies each unique vote, the county that it was cast and the candidate that was selected.  These files are large and is as challenge to summarize quickly to allow the Elections board to present the results in a quick manner. To help with this process an example of an automated script using Python was developed to present a summary of the results, which included the total votes cast, list of the candidates and the votes that they received, and identify the winner and the votes that they received.  In addition, the number of votes cast by county was also included to show the turnout in each county and identify the county with the highest voter turnout.  The results were stored in a text file containing a summary of the results that could be provided to the Elections Board

## Election - Audit Summary

Using the script that was developed we could provide a quick summary of the election results.  These results are available in the text file that we provided the Election board.

* Using the data collected in the CSV file we could determine that there were 369, 711 votes cast
* The 
Using a bulleted list, address the following election outcomes. Use images or examples of your code as support where necessary.

How many votes were cast in this congressional election?
Provide a breakdown of the number of votes and the percentage of total votes for each county in the precinct.
Which county had the largest number of votes?
Provide a breakdown of the number of votes and the percentage of the total votes each candidate received.
Which candidate won the election, what was their vote count, and what was their percentage of the total votes?
Election Results
-------------------------
Total Votes: 369,711
-------------------------

County Votes:
Jefferson: 10.5% (38,855)
Denver: 82.8% (306,055)
Arapahoe: 6.7% (24,801)
-------------------------
Largest County Turnout: Denver
-------------------------
Charles Casper Stockham: 23.0% (85,213)
Diana DeGette: 73.8% (272,892)
Raymon Anthony Doane: 3.1% (11,606)
-------------------------
Winner: Diana DeGette
Winning Vote Count: 272,892
Winning Percentage: 73.8%
-------------------------
