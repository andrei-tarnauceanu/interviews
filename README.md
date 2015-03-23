Dev Ops Interview Module
===========================

# System Troubleshooting

This system is experiencing a few problems. The command "curl http://localhost/version"
should return "0.4.6 etcd". It however does not. 

Investigate the system to uncover what the problem(s) might be. Be prepared to 
discuss what you find. 

(interviewees: set up the system with interview/devops recipe)


Two Lists
============

Given two lists, perform actions on the data. Note that both lists contain an error line, so the file format is not 100% consistent. 

# Challenges

- ** Manipulation **
Print only the name of the file and its size from both lists. 

- ** Summation **
What is the sum of the second column of each list? 

- ** Filtering ** 
Write a script that would print only the intersection of common file names from both lists. 
How many files are there associated with tasktracker? What is the total size of those files? 

- ** List Diff **
Print the file size differences between common files of both lists.  

- ** Simple Regex **
Find all the hadoop tasktracker logs that match on file name ignoring the embedded hostname. For example, hadoop-hadoop-tasktracker-ti009.log.2015-02-09 would match hadoop-hadoop-tasktracker-ti010.log.2015-02-09 because the only difference is the embedded hostname. 

- ** Complex Regex **
Convert each of the tasktracker lines in one of the list files into the following, replacing (date), (hostname) and (filename) as appropriate for the line. 
echo (hostname)@(date); scp (hostname):/var/log/(filename) . 