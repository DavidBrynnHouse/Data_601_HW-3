# David House Homework 1 due 9/17/2020

## How to Navigate this Project

---

.
* **Code** - Folder for Jupyter notebooks.
    * Cleaning_Mueller_Csv.ipynb - Jupyter notebook used to clean and organize data.
* **Data** - information both raw and cleaned
    * cleaned_mueller.csv - csv file with each individual word in its own line.
    * mueller_report.csv - The full redacted Mueller Report.
    * redactions.csv - a 2x2 csv detailing redactions of the Mueller Report.
* Executive - Analysis-of-Mueller-Report.ipynb - The main Jupyter Notebook containing the analysis for this project.
* LICENSE - MIT License
* README.md - A description of the project goals requirements and limitations.



## My goals for this project

---

The data set that I chose to work with was the full text of Special Council Robert Mueller's Report on Russian Interference in the 2016 Presidential Election. I retrieved a csv of this file from ***. By analysing this report I sought to determine what the most used words in the document were in order to see what the most important features of the investigation were. 
A large feature of the report is that much of it is redacted. For each redacted section a reason is given for the redaction so I wanted to see what the major reasons for redaction were,
Previous analysis of this document included looking at the word frequncy of the document so I wanted to specifically look for the number and type of sections that were redacted.


## Limitations and Basic Info of the Report

---

* The document is a conversion from pdf to csv format. Because of this conversion some words have been corrupted and therefore are nucountable. By visual inspection of the csv however I determined that it is not a significant amount of words that have been corrupted.
* The document has 19196 rows and 3 columns labeled page, line, and text. page and line are both integers while text contains strings


## Requirements

---

The software used in this analysis included:

1) Python
2) Pandas package for python
3) nltk package for python
