# Progress report:
## Frances Harrington, frh19@pitt.edu
## 1st Progress Report:
- Summary of what I accomplished (Keep it short (a screen-full), and provide links to related documents, including your Jupyter Notebook and data samples): 
    I have scraped the texts from the Latin Library website using a spider I built. With this data I have been able to deduce the number of texts as well as print out the textual content.
    
    ### data sharing plan:
    While I could share the full data/texts, I think that the best option for my "sharing plan" for this project is to provide the links for anyone who wishes to access the site, but not provide all of the data. The data that I will provide will be a select few of the texts that were posted by the site founder/manager himself. I would do this because while the texts are reported to be in the public domain by the site's creator/manager, he does leave the disclaimer that if there are any copyright claims he should be contacted. So, while he does seem to have done a thorough job in crediting his sources, I would ideally like to keep distribution of the texts to a minimum just in case. So, although anyone with a link can access the texts for themselves, I personally will not be responsible for distributing them.   
    
-----script notes below (copy into comments)-----

- Provide an overview of your data. Clearly document each step of your data processing pipeline.
    start requests: starts the process. Here the base url is included.-->parser for the front page: This is to extract individual author links. This includes the xpath location of each author's html then appends it onto the base url using list comprehension.-->parser to get urls for each author's individual works-->parser to scrape the actual text from each work-->store the data in an empty list

- Compile some basic stats on your data: the size and the make up are the bare minimum.

- Bullet points have their uses, but let’s see some written summaries and explanations too.

- Remember: your Jupyter Notebook file is also your presentation. Make it easy for the instructors and your classmates to understand what you are doing. Explain your goals, show your data and your processes.

- Some form of your data. If all of your data is currently stored in a git-ignored directory, make an appropriately sized samples available in a directory called data_samples.