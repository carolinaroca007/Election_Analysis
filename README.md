# Election_Analysis

## Project Overview
A Colorado Board of Elections manager, Seth, has tasked Tom, a Colorado Board of Elections employee, and I to create an algorithm to audit the election of the tabulated results for U.S. Congressional precinct in Colorado. The following tasks were accomplished and allowed us to complete the election audit.

**Tasks**
1. Calculated the total number of votes cast
2. Compiled a list of candidates who received votes
3. Compiled a list of counties who received votes
4. Calculated the total number of votes for each candidate
5. Calculated the total number of votes cast for each county
6. Calculated the percentage of votes for each candidate
7. Calculated the percentage of votes for each county
8. Defined winner of the election based on popular vote
9. Defined largest county turnout based on largest votes 

## Resources
 - Data Source: election_results.csv
 - Software: Python 3.7.6, Visual Studio Code 1.49.1

## Election Audit Results
The analysis of the election shows that:

- There were 369,711 votes cast in the election
- The candidates were:
    * Charles Casper Stockham
    * Diana DeGette
    * Raymon Anthony Doane
- The counties were:
    * Jefferson
    * Denver
    * Arapahoe
- The candidate results were:
    * Charles Casper Stockham received 23.0% of the vote and 85,213 number of the votes
    * Diana DeGette received 73.8% of the vote and 272,892 number of the votes
    * Raymon Anthony Doane received 3.1% of the vote and 11,606 number of votes
- The county results were:
    * Jefferson county received 10.5% of the vote and 38,855 number of the votes
    * Denver received 82.8% of the vote and 306.055 number of votes
    * Arapahoe received 6.7% of the vote and 24,801 number of votes
- The winner of the election was:
    * Diana DeGette, who received 73.8% of the vote and 272,892 number of votes
- The county with the largest number of votes was:
    * Denver, who received 82.8% of the vote and 306.055 number of votes

## Election Audit Summary
The script to audit election data is dynamic in which there are no hard-coded variables. If all election data is provided in the same format, in this case a .csv file, and the data elements, such as counties and candidates, are in the same order, this script will be able to execute and provide results instantly. There are a few modifications to be made even if the data elements are in the same order and format is the same; the path to the file you will be using needs to be changed. 

Example of how to path a file when you do not know the exact file path but know the name of the file you will be using for the analysis and the folder it is stored in:
        
        *file_to_load = os.path.join("Name_of_Folder", "name_of_file.csv")*

You will need to also modify the path of the file you will be saving the results to. This script prints the results to a text file, you need to alter the file name and name of the folder where you want that file to reside. You can use the follwing line of code as an example:
 
        *file_to_save = os.path.join("Name_of_Folder", "name_of_file.txt")*

If the data elements are in the same order, and the aforementioned lines of code are altered, the script will work for any other precinct elections!
