# Apriori-rule-mining
Association rule mining using Apriori algorithm implemented in Python!

We are asked to implement association rule mining using Apriori algorithm in python. The data set that we used is based on a retail market basket data obtained from an anonymous Belgian retail store. The Apriori algorithm is an influential algorithm for mining frequent itemsets for Boolean association rules. Here, frequent itemsets are the sets of items which has minimum support. The Data Structure used is a Dictionary to implement the same.

# Apriori Algorithm
First, we find the frequent itemsets, the sets of items that have minimum support. Here we need to take care that a subset of a frequent itemset must also be a frequent itemset i.e., if {AB} is a frequent itemset then both {A} and {B} should be a frequent itemset. Then, iteratively we find frequent itemsets with cardinality from 1 to k (k-itemset). At last, we use these frequent itemsets to generate association rules.
Here, frequent itemsets are generated based on minimum support defined and association rules are generated on the basis of minimum confidence. 

# Program
The functions used in this program are as follows: 
1.	runApriori: It is the main function which is applying apriori algorithm on the data set having 3 parameters namely file_data, minSupport, minConfidence which are the arguments coming from the command line.
2.	Subsets: Returns all the possible combinations of all the elements in the set.
3.	returnItemsWithMinSupport: Used to compare all the elements and return the one with Minimum support.
4.	joinSet: Used to join two different sets.
5.	getItemSetTransactionList: Used to get the transaction list of itemset.
6.	getSupport: Used to get the support of items in the itemset.
7.	printResults: Used to print the results on the console or standard output.
8.	dataFromFile: Used to read the data from the file.

# Problems Faced
Main problems faced were generating and updating frequent itemsets based on the minimum support and previous itemsets. Also, keeping a track of the changes was  difficult. First, the data structure list was used in place of a dictionary but retrieving data items became problematic and therefore in the end Dictionary was used. This made it possible to retrieve data on the basis on key value pairs.
