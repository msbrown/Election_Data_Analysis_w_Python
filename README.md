## Introduction to using Python for Analyzing Election Data

Welcome to the code repository for the workshop **A Gentle Introduction to using Python for Analyzing Election Data** These notebooks are meant for those comfortable with data analysis concepts and have used a spreadsheet program like Excel to analyze election data but who want to get a sense of the power of Python to analyze larger (i.e., 5 million or more records) datasets and scrape data from parties, election commission's social media pages. The goal is to give you some concrete examples for getting started with Python and Pandas (and maybe overcome some of the intimidation of code). A tutorial based on these notebooks was given at the Data Academy for the <a href="http://openelectiondata.net/en/">Open Election Data Initiative</a>, an initiative that promotes accountability in elections through the use of open election data.

## Requires Anaconda (Python version 2.7) Installation   
Before you can download and use the notebooks, I recommend you install <a href="https://www.continuum.io/downloads">Anaconda (Python version 2.7)</a> on your computer. Anaconda comes with most of the libraries you'll want to use with Python.

## To Start the Notebooks
Once you have Anaconda installed, you need a little bit of command line fun to get things up and running.

<br>1. Download the attached files, uncompress them and note where the unzipped folder is located.
<br> 2.
WINDOWS: Open up a command prompt window (Type cmd in windows search and hit return and it usually opens a new black window).
MAC: Open a new window in Terminal.
<br> 3. In that new window, type: ``cd <location of where the file is saved>`` and hit return. So for example, if I saved the file in my documents folder, then the command I will type will look like this:
``cd c:\Users\mbrown\documents\``
Basically what you are doing there is Changing the Directory (hence "cd") to the folder where you saved the files.
<br> 4. WINDOWS: Next type this in the command prompt and hit return: ``dir``
MAC: Next type this in the terminal and hit return: ``ls``
<br> 5. You should then get a list all the files and folder in that directory so you can confirm the files located there are the same as here.
<br> 6. At the new prompt, we're going to tell it to launch Jupyter notebooks by typing the following and then hitting return: ``jupyter notebook``
<br> 7. Some things should log in the command prompt window and then it should automatically launch a new webpage in your default browser (usually at this address: <a href="http://localhost:8888/tree"> http://localhost:8888/tree</a>).
<br> 8. In that new browser window, click the file called 01 - Python and Pandas-Introduction.ipynb and hopefully it will launch a new tab with that file.
<br> 9. Go through the notebook and run the code by highlighting the cell block and hitting run (->).
<br> 10. Enjoy. I highly suggest you make a copy of a notebook and then just try modifying the parts with the code. Think about what might break it and then do so. Tinker with the code and change some of it (especially some of the code in red as those are usually variables).

## Table of Contents

* [Notebook 1: 01 - Introduction to Python and Pandas](https://github.com/msbrown/Election_Data_Analysis_w_Python/blob/master/01%20-%20Python%20and%20Pandas-Introduction.ipynb)
 <br> Introduction to DataFrames, viewing and filtering data, renaming and dropping columns, and quick pivot tables.
* [Notebook 2: Python and Pandas- Summarizing Voter List Data](https://github.com/msbrown/Election_Data_Analysis_w_Python/blob/master/02%20-%20Python%20and%20Pandas-Summarizing%20Voter%20List%20Data_v1.7.ipynb)
 <br> Combining three Comma-Separated files (CSV) into 1 master file, demonstrating how efficiently Python handles a large (millions of records) dataset. Then a quick tour through common tasks you perform on a voter list: Determining duplicates, summarizing the data at a higher (geographic) level and saving that dataset for analysis in a spreadsheet program. Also a quick bit on histograms (plots).
* [Notebook 3: Optional: Dealing with Dates in a Voter_List handling_dates](https://github.com/msbrown/Election_Data_Analysis_w_Python/blob/master/03%20-%20Extra-Voter_List--handling_dates.ipynb)
  <br> Some extra notes to help you troubleshoot dates (in Voter Lists). Takes a variable like the birthdate which may be stored as an (incorrect) data type and convert it to the proper date format for analyzing so you can calculate age based on a specified date (e.g., election day).
* [Notebook 4: 04 - Facebook Public Page/Group Scraper](https://github.com/msbrown/Election_Data_Analysis_w_Python/blob/master/04%20-%20Facebook_scraper_v4.ipynb)
  <br> This notebook advises you to create a Facebook App ID & Secret. Then it uses that information and Facebook's Graph API (v 2.6) to scrape all the posts and comments of a Facebook *Public* Page (or Group). It also captures the related metadata, including post message, post links, and counts of each reaction on the post. All this data is exported as a CSV, so it can be imported into an analysis program like Excel.

### Data folder

  Although I don't recommend keeping your data in a repository, I have done it here for the purpose of our shared use. In the data directory you'll find 2 of the examples used in the notebooks. For notebook 02 (voter list), you'll need to download the three larger files from the dropbox link provided in that notebook and save them in your data folder (they were too large to host on github).

### Coming soon
I plan to add at least two more notebooks for scraping data from Twitter accounts. Please let me know if you have other needs or ideas.

### Corrections, Questions, or Suggestions?
If you find any issues in these code examples, feel free to submit an Issue or Pull Request. Or reach out to me on Twitter <a href="https://twitter.com/animatedroamer">@animatedroamer</a> or here on GitHub.

### Credits and Many Thanks
This series of notebooks was originally inspired by <a href="https://github.com/GusSand/itp_talk_2016">Gustavo Sandoval and his ITP Camp session</a> where he gave a lovely overview of the Pandas library. In creating the notebooks I also relied heavily on, and was inspired by,  <a href="https://github.com/jackiekazil/data-wrangling">Jackie Kazil's code</a> and great book (and video series) Data Wrangling with Python. The Facebook scraper is really just <a href="https://github.com/minimaxir/facebook-page-post-scraper">Max Woolf's</a> code in a notebook format.
<br>The idea to include it here comes from a great suggestion by <a href="https://github.com/lisoffsky">Mr. Lisovsky</a> that election monitoring organizations are often trying to track what events campaigns are having (and where) and that the scraper might make it easier for them.
