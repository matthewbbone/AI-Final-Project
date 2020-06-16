New Jersey News Cleanup
Matthew Bone

Vision: 
This project is a preliminary cleanup of the data that is to be used in a research project by Professor Holcomb from the English department. Professor Holcomb is teaming up with a group at Montclair State's Center for Cooperative Media to map the local news ecosystem of New Jersey. In particular, they want to use this dataset to map the geographic spread of news stories in the state. They collected this data in partnership with the Internet Archive (https://archive.org/index.php) by scraping all of the text data from over 700 news sites in New Jersey, including social media such as Facebook and Twitter. However, during this web scraping, many unuseable webpages were scraped. For instance, there are Facebook login pages and "About Us" pages from news sites. Therefore, in this project I try to create a classifier that will be able to separate the useable data from the unuseable data.

In this project I try four different ways to correct for imbalanced classes in the data and I add URL and domain features to see if the neural net classifiers improve. 

Modules:
This project's architecture is very simple, all of the relevant code is contained in the report.ipynb document. Running it would only require pressing "run all" in a python notebook. However, since I cannot share the data, this is not possible.

How to Run: 
The data that was used to run this report is not owned by the author and hence it cannot be shared without the relevant permissions. However, the results of the most recent grid search runs can be found here https://docs.google.com/spreadsheets/d/1qVNPxp4vlo7M2kG1qsRwlHz8O6PK8bNTq1OOVTl_LgI/edit?usp=sharing. Using these, one can reproduce most of the analysis between model groups and recreate the best model.  

UPDATES SINCE WALKTHROUGH
Most of my work was done by the time of the walkthrough. However I did make a few changes and added most of the commentary after the walkthrough as well as a few other things:
1. improved in-line documentation for helper functions
2. Reformatted the results of the top model for easier understandability
3. fixed the to_csv calls which were inadvertantly saving only recall_results
4. Reran grid search for the URL model group due to not saving it as a csv (due to point 3) so that I could rerun the final top model