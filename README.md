# Apache-Spark-Implementations
The file contains four sub-tasks related to a project for my postgraduate course.

**1)** A MapReduce program, a variation of the word-count problem, is implemented to create and count "numeronyms." Numeronyms correspond to words such as the following:
s5n – shorten, 
h7k – hyperlink,
l10n – localisation,
i18n – internationalization.
The numeronym of a word is defined as the alphanumeric string formed by taking the first and last characters of the word and inserting the number of characters between the first and last characters. More specifically, it takes into account words with a length of 3 characters or more, creates numeronyms, and then prints the number of occurrences of each.
The program ignores:
● words shorter than 3 characters
● punctuation marks
● upper/lower case letters, i.e. it is case-insensitive
For this sub-task,  the file SherlockHolmes.txt is used as input.

**2)** The sub-task implements a variation of the word-count problem using Spark. First, the program reads a text file, deletes all punctuation marks, and converts all characters to lowercase.
Τhen calculates the average length of words beginning with a specific character (a-z) and sorts the results according to the average, displaying the letters with the highest average first.
The result of the execution is a list of letters (the first letter of each word) followed by the corresponding average length of words beginning with that letter. 
For example:
k 8.2,
a 5.6,
b 4.8,
f 4.5,
For this sub-task,the file SherlockHolmes.txt is used as input.


**3)** A program that calculates the number of occurrences of consecutive 2s, 3s, and 4s in the above DNA sequence for each line of the input file. The processing of one line is independent of the others. For this sub-task, i used the file ecoli.txt as input.


**4)** Our data source is a CSV file (each line corresponds to a tweet) containing Twitter comments about airline services in the following format:
● tweet_id
● airline_sentiment
● airline_sentiment_confidence
● negativereason
● negativereason_confidence
● airline
● name
● text
● tweet_created
● user_timezone.
A program is created using Spark Dataframes to answer various questions. For this sub-task,the file tweets.csv is used as input. 
