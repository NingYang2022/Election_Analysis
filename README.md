# Election Analysis
## <font color=#6495ED>Overview of Project</font>
A Colorado Board of Elections employee has given you the following tasks to complete the election audit of a recent local congressional election.
### <font color=#6495D>Purposes</font>

* Calculate the total number of vote cast.
* Get a complete list of counties where received votes.
* Calculate the total number of votes each county received.
* Calculate the percentage of votes each county won.
* Determine the county with the highest turnout.
* Get a complete list of candidates who received votes
* Calculate the total number of votes each candidate received.
* Calculate the percentage of votes each candidate won.
* Determine the winner of the election based on popular vote.



---
## <font color=#6495ED>Election Audit Results</font>
The analysis of the election show that
- There were 369,711 votes cast in the election

- The county results were:
    * Jefferson received 10.5% of the vote and 38,855 of votes

    * Denver received 82.8% of the vote and 306,055 of votes

    * Arapahoe received 6.7% of the vote and 24,801 of the votes

- The county with the highest turnout was: 
    * Denver received 82.8% of the vote and 306,055 of votes

- The candidate results were:
    * Charles Casper Stockham received 23.0% of the vote and 85,213 of votes

    * Diana DeGette received 73.8% of the vote and 272,892 of votes

    * Raymon Anthony Doane received 3.1% of the vote and 11,606 of the votes

- The county with the highest turnout was:
    * Diana DeGette received 73.8% of the vote and 272,892 of votes


![election_results_terminal_snapshot](https://github.com/NingYang2022/Election_Analysis/blob/main/Resources/election_results_terminal_snapshot.png?raw=true)

![election_results_text_file_snapshot](https://github.com/NingYang2022/Election_Analysis/blob/main/Resources/election_results_text_file_snapshot.png?raw=true)


## <font color=#6495ED>Election Audit Summry</font>
This script can be used for any other election with some modifications.
For example:
1.	We can import data from other elections by modifying the name of the file. 
In the script, we could replace <code>("Resources", "election_results.csv")</code> with different path and file name.

```
 # Add a variable to load a file from a path.
file_to_load = os.path.join("Resources", "election_results.csv")

```

2. After we inspect the source csv file, we could retrieve the names of candidates and counties by re-defining the indexes of the loop variable <code>row[]</code> to reference the candidate colume and county colume.
```
# Get the candidate name from each row.
        candidate_name = row[2]

# Extract the county name from each row.
        county_name = row[1]
```
