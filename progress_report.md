# Progress report:
## Frances Harrington, frh19@pitt.edu
## 1st Progress Report:
### 3/5/2021

   ## Summary of what I have accomplished as well as what I will do next:
   I have scraped the texts from the Latin Library website using a [spider](http://localhost:8888/notebooks/Documents/ling1340/Latin-Vocabulary-Analysis/LatLibSpider.ipynb) I built. With this data I have been able to deduce the number of texts as well as print out the textual content and titles. Once I constructed my spider, I appended the data to empty lists which I then converted to Series in order to put them into a DataFrame. This DataFrame right now consists of the titles and their corresponding texts. After building this DataFrame I pickled it and saved it to my data folder, which is included in the .gitignore. I also have a sample of ten files pickled in the [data_samples](http://localhost:8888/tree/Documents/ling1340/Latin-Vocabulary-Analysis/data_samples) folder.
    I was able to extract the urls of each author and work by using multiple parse functions and xpath notation as well as list comprehension. The list comprehension was used in the second parser to add the new path onto the base url. Through this process I learned a lot about spiders and the way that they are constructed as well as how to use them. 
    Currently I have not done any analysis on this data. I have fetched the information from the Latin Library website, put that information into the DataFrame, and pickled that Dataframe. Next I will focus on building more information into the preexisting DataFrame (i.e. URLs, genres, style) as well as diving into the analysis portion. Because I have collected data from many different eras it might also be relevent to include era (pinpointing exact years are difficult with the more ancient texts) in the analysis/DataFrame.
    
   ## Data sharing plan:
   While I could share the full data/texts, I think that the best option for my "sharing plan" for this project is to provide the links for anyone who wishes to access the site, but not provide all of the data. The data that I will provide will be a select few of the texts that were posted by the site founder/manager himself. I would do this because while the texts are reported to be in the public domain by the site's creator/manager, he does leave the disclaimer that if there are any copyright claims he should be contacted. So, while he does seem to have done a thorough job in crediting his sources, I would ideally like to keep distribution of the texts to a minimum just in case. So, although anyone with a link can access the texts for themselves, I personally will not be responsible for distributing them.   

## 2nd Progress Report:
## 3/23/2021
   ## Summary of what I've accomplished and what I'll do next: 
   So far I've completed my data acquisition process. I cleaned the data that I got from my Spider and saved it as strings into a DataFrame (which I pickled and saved into my data folder). Along with the text and titles, the DataFrame also contains the tokenized text and token counts. I re-saved my data samples as a csv instead of as a .pkl for easier viewing--[here](https://github.com/Data-Science-for-Linguists-2021/Latin-Vocabulary-Analysis/tree/main/data_samples). 
   Once all of my data was saved and pickled I created a new Jupyter Notebook file for my analysis portion, seperate from my Spider so that I wouldn't have to wait too long everytime I needed to re-run all the cells. [This](https://github.com/Data-Science-for-Linguists-2021/Latin-Vocabulary-Analysis/blob/main/AnalysisCode.ipynb) file is dedicated to my analysis. I have begun to work on the linguistic analysis of my data. I got some basic information on the data (shape, token count stats, .info()) and then began to work on the rest. The linguistic analysis that I've done is very surface level, I have compiled the works in which each word (and its various forms) appears. Next I will begin to sort the data by genre and style. I also have some ideas about running analysis on adjectives that describe each of these nouns, but I will have to see down the road how that works out.
   
   ## Data sharing plan:
   My data sharing plan is the same as discussed in my first progress report: I will provide the links to the website but I will only directly provide a small set of data samples.
  
   ## Licensing:
   For my license I decided on an MIT license. I chose this license because it is a very open, short, and simple license. I want anyone to be able to do whatever they want with this data/project if they so choose and this license allows for that. 
