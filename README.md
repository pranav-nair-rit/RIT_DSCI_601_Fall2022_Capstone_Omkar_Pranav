# RIT_DSCI_601_Fall2022_Capstone_Omkar_Pranav
Data Science Capstone Project

Problem Statement:
	Reduce the time taken for assigning the reviewers for the Github PR.

Solution:
	Develop the logic which can recommend reviewers in the ranking order. Most suitable reviewer will have rank 1.

Step 1 :
		To understand Ranking problem we decided to use the dummy data and train the model which gives the output as a ranking output. 
		Code Folder : Ranking_Problem
		Code File : RankingDevelopersForRefactoring.ipynb
		Data File :  project3-authors.csv


	Instructions to run program file :	
		1.  To run ‘RankingDevelopersForRefactoring.ipynb’ program kindly use the Jupyter notebook. All the cells are aligned on order so you will just need to run all the cells at one time.
		2. This programs might take more than a 6 hrs to run completely. We have trained the same using the 	RIT servers.

	By developing this code we understood how ranking problem works.

Step 2 :
		In our study we found that there are multiple techniques to get the ranking solution using different techniques. Where hyper graph technique was the prefect fit for our problem. 
	
		Normal graph can not show the relationship between more than two nodes at same time. 	Which is possible in terms of hyper graph database. Using hyper graph we can show the relationship between multiple reviewers with respect to same PR. This is the reason why we choose to go with hypergraph algorithm. 

	Inputs for Hypergraph : PR request ID, PR comments, Reviewers
	
Step 3: 
		We decides to get all real work data from open source GitHub project for Hypergraph implementation. 
	To achieve this we have used GitHub API which is developed by the GitHub itself. The code of implementation	of API is implemented in Folder Real_World_Data_Extraction.
		Code Folder : Real_World_Data_Extraction.
		Code File : Data_Mining.ipynb
		Data Retrieved File : reviewers.bin 

	
	Instructions to run program file:
		1. Use Jupyter notebook to run ‘Data_Mining.ipynb’ file.  
		2. All the cells are managed in order to run. So we can directly run all the cells.
		3. Downloading of data might take time depending on the internet and API speed.
		4. Pickle file I been saved in the same folder so as to use that data in future while developing the hypergraph.



Future Implementation :
	Develop the code for hypergraph using the reference of Graph code available on the internet. 
