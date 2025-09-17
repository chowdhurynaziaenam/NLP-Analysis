## NLP analysis

A comprehensive repository which performs several NLP analyses scraping Wikipedia pages for 6 Marvel Comic characters.

## Table of Contents

* [General overview](#general-overview)
* [Environment](#environment)
* [Libraries & Packages](#libraries-&-packages)
* [Results](#results)
* [Setup](#setup)
* [Acknowledgement](#acknowledgement)

## General Overview

This project scrapes Wikipedia Pages for 6 Marvel comic characters- Iron Man, Spider-Man, Hulk, Captain America, Thor (Marvel Comics), and Bucky Barnes. It calculates the popularity Score using a weighted sum of metrics such as word count, page text size, number of headings, images, tables, infobox size, internal wiki links, section depth, category count etc. It also identifies the adjectives associated with each character to determine their key personality traits. Using TF-IDF (Term Frequency-Inverse Document Frequency) Analysis, here the most distinctive keywords associated with each character was identified. The TF-IDF score is a numerical value that increases when a word appears frequently in a document, and decreases when the same word appears in many documents. Based on the score, character cluster analysis is performed. It also shows the most commonly mentioned entities i.e., people, organizations, work of art, and locations in relation to each Marvel character from their Wikipedia article. It further analyses the emotional tone of character descriptions and extracts the most positive and negative sentences. It interprets the sentiment using TextBlob tool showing Polarity, Subjectivity, and Mentioned Polarity.

•	Polarity: It shows the sentiment of a text ranging the value between -1 (very negative) to 1 (very positive) where 0.0 is neutral sentiment.

•	Subjectivity: It shows article subjectivity referring to how personal or opinion-based the text is. The value of it ranges between 0 (objective) to 1 (very subjective).

•	Mentioned Polarity: It refers to the explicit sentiment attached to a particular entity mentioned in the text.

Finally, it generates Trait-based Word cloud and visualizes the traits or adjectives for each Marvel comic character.

## Environment

The project was executed using Google Colab.

## Libraries & Packages 

Web scraping: 

-beautifulsoup (from bs4 package): For extracting raw text data from websites (Wikipedia pages) for further NLP processing.

Natural Language Processing (NLP) Libraries

-nltk (Natural Language Toolkit): For tokenization
-textblob: For sentiment analysis, phrase extraction
-spacy: For entity recognition

Data visualisation, manipulation, and analysis
-NumPy: For numerical operations
-Matplotlib: For plotting graphs
-Pandas: For data manipulation and analysis
-Scikit-learn (sklearn)
  

## Results

Based on popularity score using a weighted sum of metrics, Hulk is obtained as the most popular character. Depending on the TF-IDFcharacter, characters are clustered into 2 clusters using K means where Cluster 0 includes Spider-Man, Hulk, Thor, and Cluster 1 includes Iron Man, Captain America, Bucky Barnes. 
Spider-Man has a polarity of 0.127, so most mentions of him are mildly positive. Iron Man has a subjectivity of 0.447, meaning about 44.7% of the texts are opinion-based and polarity of 0.068 indicating mildly positive. Texts in Bucky barnes have least positive sentiment and appear as most neutral context.
It also generates Trait-based Word cloud and visualizes the traits or adjectives for each Marvel comic character as follows:

Top traits wordcloud text for Iron Man: American American American American American American  comic comic comic comic comic comic  own own ...

Top traits wordcloud text for Spider-Man: American American  comic comic comic comic comic comic comic comic comic comic comic comic comic com...

Top traits wordcloud text for Hulk: American  comic comic comic comic comic comic comic comic  dissociative dissociative dissociative...

Top traits wordcloud text for Captain America: American American American American American American American American American American American A...

Top traits wordcloud text for Thor: American American  comic comic comic comic  own own own  same same  many many many  mythological myt...

Top traits wordcloud text for Bucky Barnes: other  second  original  further  guilty  new new new  formidable  bionic  S.H.I.E.L.D.  former  tee...


## Setup

* Open Google Colab
* Upload the notebook or open it directly from Google Drive
* Ensure all required packages are installed
* Run the cells sequentially to execute the analysis

## Acknowledgement

This project includes content from the following Wikipedia pages:

- [Iron Man] ('https://en.wikipedia.org/wiki/Iron_Man')
- [Spider-Man] ('https://en.wikipedia.org/wiki/Spider-Man')
- [Hulk] ('https://en.wikipedia.org/wiki/Hulk')
- [Captain America] ('https://en.wikipedia.org/wiki/Captain_America')
- [Thor] ('https://en.wikipedia.org/wiki/Thor_(Marvel_Comics)')
- [Bucky Barnes] ('https://en.wikipedia.org/wiki/Bucky_Barnes')

Content from these articles is licensed under the [Creative Commons Attribution-ShareAlike 4.0 International License (CC BY-SA 4.0)](https://creativecommons.org/licenses/by-sa/4.0/).










