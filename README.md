# Election Summary Using PyPoll

## Overview

###
This project was developed to create the PyPoll tool using Python script to automate the process of auditing the votes and provide a summary that can be submitted to the Elections Commission.  The data for each polling location is stored in a comma separated value (CSV) file which identifies each unique vote, the county that it was cast and the candidate that was selected.  These files are large and is a challenge to summarize quickly to allow the Elections Commission to present the results in an efficient manner.  To help this process an example of an automated script using Python was developed to present a summary of the results, which included the total votes cast, list of the candidates and the votes that they received and identify the winner and the votes that they received. In addition, the number of votes cast in each county was added to the PyPoll tool to show the turnout in each county and identify the county with the highest voter turnout. The results were stored in a text file containing a summary of the results that could be provided to the Elections Commission.

---

## Election - Audit Results
###
Using the script that was developed we could provide a quick summary of the election results.  These results are available in the [text file](analysis/election_analysis.txt) that we provided the Election Commission.

* Using the data collected in the CSV file we could determine that there were 369, 711 votes cast
  -The was calculated by calculating the total entries contained in the file which represented a single vote
  -The code ran a loop reading each row of the file individually
  code image
* Based on the audit the following results for each county are as follows:
  - Jefferson: 10.5% (38,855)
  - Denver: 82.8% (306,055)
  - Arapahoe: 6.7% (24,801)
* From this we can observe that Denver County had the greatest voter turnout at 306,055 making up 82.8% of the total vote
* From the candidates in the election the following results were collected:
  - Charles Casper Stockham received 23.0% of the vote with a total of 85,213 votes.
  - Diana DeGette received 73.8% of the vote with a total of 272,892 votes.
  - Raymon Anthony Doane received 3.1% of the vote with a total of 11,606 votes.
* Based on the results the winner of the congressional election was:
  - Diana DeGette with a total of 272,892 votes with a total of 73.8% of the vote.

The results of the congressional election were calculated using loops to identify the candidate and the county that each vote was cast. The results were collected and written into the election analysis document that summarized the votes for each candidate and the counties that the votes were cast.  This automated audit of the results rapidly provides a summary that can be submitted for the Election Commission.  

To illustrate how the use of PyPoll for the evaluation of voting results, this section looks at the key elements that were incorporated into the program that is being proposed. To organize the data for analysis, variables for the values to be summarized were characterized as lists and dictionaries as needed to store and organize the data as it is being compiled.

![Coding image for variable identification]"Resources/Code_County_Variables.png"

With the variables defined we could iterate through the election CSV file and store the voting data as the program reads each row of the data.  This allowed the data to be stored in the dictionaries where if could be accessed.
![Coding image for CSV iteration]"Resources/Code_County_Data_Collection.png"

Finally, the data was extracted and inserted into strings to be added to the text files and displayed within the terminal prompt.  This provides the summary that can be presented to the Elections Commission.

![Coding image for data extraction]"Resources/Code_County_Data_Extract.png"

---
## Election - Audit Summary

### Expansion of use

The use of this script to automate the audit and analysis of the voting results give the Election Commission a tool to provide quickly gather the results of the election which can be presented and shared using the summary provide with the election analysis summary text file. This file can be used to share the results in a timely manner.  This code can be used across other election to complete the audit of the results and analyze the results to provide the winner and the distribution of the votes between the candidates and the counties where the votes were cast.  This can be expanded across other elections and provide the summary of results for each.  The data can be used to track voter turnout over time and provide information that can be used by election commission to share the findings.

### Added Features

To facilitate the expanded use of the PyPoll for other elections and providing the election commission with and analysis and audit of the results.  To share with the election commission some other functions that could be incorporated into PyPoll to expand its use.  

1. Customize the file naming to allow for expanded use of the data being collected

By adding date and filename tags into the automated file naming of the text files that contain the summary of data, it will allow for an imbedded reference to the source and time of the analysis. Including this functionality can help organize the file containing the analysis of the results allowing them to be stored and easily referenced for future use.


2. Include the breakdown of voting results per county based on the results.  

In its current form, the PyPoll programs provides the summary of the overall voting for the 3 counties.  Further expansion of this analysis can include county specific results that can be used for a deeper analysis of the voting data. This added functionality will show the votes for each candidate as seen in each county in the election. This can be used to show trends within the county and provide the Elections Commission more insight into voting trends at a county level. This shows the flexibility of the program and how it can be expanded to include other functions as needed by the Elections Commission.







