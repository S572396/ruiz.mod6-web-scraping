# Web Scraping and NLP with Requests, BeautifulSoup, and spaCy

## Introduction: This repo will work with url "https://web.archive.org/web/20210327165005/https://hackaday.com/2021/03/22/how-laser-headlights-work/"
## Sentences, words, text will be analyzed with filtering by tokens and lemmas and viewing scores. 
## Histograms for the scores of tokens and lemmas will be created.

Complete the tasks in the Python Notebook in this repository.
Make sure to add and push the pkl or text file of your scraped html (this is specified in the notebook)

## Create and activate a virtual environment. Run the following commands - or similar ones as needed -  to install these into your virtual environment:

! pip install matplotlib  ## pre question
install ipkernel ## pre question
python -m spacy download en_core_web_sm ## for question 3
python -m pip install beautifulsoup4
python -m pip install html5lib
python -m pip install requests
python -m pip install spacy
python -m pip install spacytextblob
python.exe -m pip install --upgrade pip


#### Create and activate a Python virtual environment. Before starting the project, try all these imports FIRST. Address any errors you get running this code cell 
#### by installing the necessary packages into your active Python environment. Try to resolve issues using your materials and the web.
#### If that doesn't work, ask for help in the discussion forums. You can't complete the exercises until you import these - start early! 
#### We also import pickle and Counter (included in the Python Standard Library).

from collections import Counter
import pickle
import requests
import spacy
from bs4 import BeautifulSoup
import matplotlib.pyplot as plt

!pip list

print('All prereqs installed.')# Create and activate a Python virtual environment. 

#### before Question 1 created sentences_list txt file to view all sententences and aid visually

#### Queston 3 python -m spacy download en_core_web_sm in virtual env.

#### Question 5-feed the first sentence if does not find.

#### Question 6-print to text file: scores_list.txt created to view each sentence score


## Rubric

* (Question 1) Article html stored in separate file that is committed and pushed: 1 pt
* (Question 2) Article text is correct: 1 pt
* (Question 3) Correct (or equivalent in the case of multiple tokens with same frequency) tokens printed: 1 pt
* (Question 4) Correct (or equivalent in the case of multiple lemmas with same frequency) lemmas printed: 1 pt
* (Question 5) Correct scores for first sentence printed: 2 pts (1 / function)
* (Question 6) Histogram shown with appropriate labelling: 1 pt
* (Question 7) Histogram shown with appropriate labelling: 1 pt
* (Question 8) Thoughtful answer provided: 1 pt
