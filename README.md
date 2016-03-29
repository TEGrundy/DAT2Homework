# DAT2Homework
DAT2 Homework Storage

##Homework Details
1. Look at the head and the tail of chipotle.tsv in the data subdirectory of this repo. Think for a minute about how the data is structured. What do you think each column means? What do you think each row means? Tell me! (If you're unsure, look at more of the file contents.)
2. How many orders do there appear to be?
3. How many lines are in this file?
4. Which burrito is more popular, steak or chicken?
5. Do chicken burritos more often have black beans or pinto beans?
6. Make a list of all of the CSV or TSV files in the GA-SEA-DAT1 repo (using a single command). You will be working on your local repo on your laptop. Think about how wildcard characters can help you with this task.
7. Count the approximate number of occurrences of the word "dictionary" (regardless of case) across all files in the GA-SEA-DAT1 repo.

Optional: Use the the command line to discover something "interesting" about the Chipotle data. Try using the commands from the "advanced" section!

##Answers
1.This data appears to be a listing of orders with a several descriptive columns. Order_id (pk), quantity, item_name, choice_description, item_price. Commands used:
  a. head chipotle.tsv
  b. tail chipotle.tsv
   
2. There appears to be 1834 order ids. Commands Used:
  a. sort chipotle.tsv
  b. head chipotle.tsv
  c. tail chipotle.tsv
3. There are 4623 lines in this file. Commands Used:
  a. wc -l chipotle.tsv
4. Chicken burritos are more popular than steak burritos. Commands Used: 
  a. grep -c -i "steak burrito" chipotle.tsv
  a. grep -c -i "chicken burrito" chipotle.tsv
5.
6
7.~ 85 occurrences of dictionary. Commands Used: 
  a. grep -r -i "dictionary" . > dictcount.csv
  b. grep -c -i "dictionary" dictcount.csv
7. 
